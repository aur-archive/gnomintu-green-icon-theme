# Maintainer: GreenRaccoon23 <GreenRaccoon a t gmail d o t com>

_pkgname=gnomintu-green
pkgname=gnomintu-green-icon-theme
pkgver=0.r0.6ecca5a
pkgrel=2
pkgdesc='Fusion of Mint-X, GNOME, Ubuntu-Mono, and Humanity icon themes (green ubuntu folders)'
arch=('any')
url="https://github.com/GreenRaccoon23/$_pkgname"
license=('GPL3')
makedepends=('git' 'intltool' 'librsvg' 'gtk-update-icon-cache')
install="$_pkgname.install"
source=("$pkgname"::"git+https://github.com/GreenRaccoon23/$_pkgname.git")
md5sums=('SKIP')

pkgver() {
	cd "$srcdir/$pkgname"
	printf "0.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	cd "$srcdir/$pkgname"
  	install -dm 755 "$pkgdir"/usr/share/icons/gnomintu-green
  	cp -drf --no-preserve='ownership' . "$pkgdir"/usr/share/icons/gnomintu-green/

}