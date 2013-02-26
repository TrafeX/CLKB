== Build new package ==
<pre>
dh_make -s --indep --createorig  --email code@trafex.nl --copyright=gpl3

# Remove make calls
grep -v makefile debian/rules > debian/rules.new
mv debian/rules.new debian/rules

# debian/install must contain the list of scripts to install
# as well as the target directory
echo clkb usr/bin > debian/install

# We don't want a quilt based package
echo "1.0" > debian/source/format

# Remove the example files
rm debian/*.ex

# Build the package.
debuild -us -uc

# Build with signing
debuild -k99C7BA1C

export DEBFULLNAME='Tim de Pater'
export DEBEMAIL='code@trafex.nl'

# Create changelog
debchange --create --package clkb -v 1.0.0-BETA2

# Release changelog
debchange -r
</pre>

== Release new version ==
<pre>
debchange -v 1.0.0
debchange -r
export DEBFULLNAME='Tim de Pater'
export DEBEMAIL='code@trafex.nl'
debuild -us -uc
debuild -k99C7BA1C
</pre>


== Resources ==

* http://askubuntu.com/questions/27715/create-a-deb-package-from-scripts-or-binaries
* http://ghantoos.org/2008/10/19/creating-a-deb-package-from-a-python-setuppy/
