#! /bin/sh
# Maintainer: Jorge <jorge.barroso.11@gmail.com>
pkgname=extra-fonts-gimp
pkgver=1.0
pkgrel=4
pkgdesc="Extra web fonts for the Gimp"
arch=('any')
url=("http://www.urbanfonts.com/free-fonts.htm" "http://www.dafont.com/new.php")
license=('GPL')
depends='gimp'
install=extra-fonts-gimp.install
source=('http://rs469p11.rapidshare.com/cgi-bin/rsapi.cgi?sub=download&fileid=2473143703&filename=fonts.tar.gz&dlauth=0123456789')

package() {
cd "${srcdir}"

mkdir -p "${pkgdir}/usr/share/gimp/2.0/fonts"
cp -r -p "${srcdir}/fonts"/* "${pkgdir}/usr/share/gimp/2.0/fonts"

sed 's|usr/local|usr|' -i "${pkgdir}/usr/share/gimp/2.0/fonts"/*/*

}

# vim:set ts=2 sw=2 et:

sha512sums=('5ba56a033e9b5d65466cea490dd1ef3d87142ee6cb77c1aa1579026544293f3acf992b7af1cf9ed1bfd2cecfe4d3929f35accfb3f0d7de4f04023b63640b6dd0')
