# Maintainer: Brenton Horne <brentonhorne77 at gmail dot com>

_pkgname=Shadow
pkgname=shadow-icon-theme
pkgver=2.2.1
pkgrel=1
arch=('any')
pkgdesc="A flat colourful icon theme for GNOME 3.10+"
makedepends=('git')
url="http://gnome-look.org/content/show.php/${_pkgname}?content=170398"
source=("git+https://github.com/rudrab/${_pkgname}.git#tag=v${pkgver}")
license=('GPL')
sha256sums=('SKIP')

pkgver() {
  cd $srcdir/${_pkgname}
  git describe --tags `git rev-list --tags --max-count=1` | sed 's/v//g'
}

package() {
  mkdir -p $pkgdir/usr/share/icons/
  cp -a "$srcdir/${_pkgname}" "$pkgdir/usr/share/icons/${_pkgname}"
  cd $pkgdir/usr/share/icons/${_pkgname}/scalable/places/
  ln -sf distributor-logo-archlinux.svg start-here.svg
}
