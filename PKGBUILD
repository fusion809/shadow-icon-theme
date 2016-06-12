# Maintainer: Brenton Horne <brentonhorne77 at gmail dot com>

_pkgname=Shadow
pkgname=shadow-icon-theme
pkgver=1.7.9.6
pkgrel=1
arch=('any')
pkgdesc="A flat colourful icon theme for GNOME 3.10+"
url="http://gnome-look.org/content/show.php/${_pkgname}?content=170398"
source=("https://github.com/rudrab/${_pkgname}/archive/v${pkgver}.tar.gz")
license=('GPL')
sha256sums=('fce813054a4729de7a14f20c4373c73056a6029c503b3c7d79493e671b79cc32')

package() {
  mkdir -p $pkgdir/usr/share/icons/
  cp -a "$srcdir/${_pkgname}-${pkgver}" "$pkgdir/usr/share/icons/${_pkgname}"
}
