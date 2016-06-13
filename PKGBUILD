# Maintainer: Brenton Horne <brentonhorne77 at gmail dot com>

_pkgname=Shadow
pkgname=shadow-icon-theme
pkgver=2
pkgrel=1
arch=('any')
pkgdesc="A flat colourful icon theme for GNOME 3.10+"
url="http://gnome-look.org/content/show.php/${_pkgname}?content=170398"
source=("https://github.com/rudrab/${_pkgname}/archive/v${pkgver}.tar.gz")
license=('GPL')
sha256sums=('83ca95c73379eb772a98eca5514c546d01b53444e984ffb67db3cf7983883a85')

package() {
  mkdir -p $pkgdir/usr/share/icons/
  cp -a "$srcdir/${_pkgname}-${pkgver}" "$pkgdir/usr/share/icons/${_pkgname}"
  cd $pkgdir/usr/share/icons/${_pkgname}/scalable/places/
  ln -sf distributor-logo-archlinux.svg start-here.svg
}
