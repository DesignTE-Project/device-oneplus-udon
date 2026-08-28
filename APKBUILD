# Reference: <https://postmarketos.org/devicepkg>
maintainer=""
pkgname=device-oneplus-udon
pkgver=1.0.0
pkgrel=0
pkgdesc="OnePlus Ace 2"
url="https://postmarketos.org"
arch="aarch64"
license="MIT"
depends="
	android-tools-mkbootimg
	linux-oneplus-udon
	postmarketos-base
	"
makedepends="devicepkg-dev"
source="
	deviceinfo
	modules-initfs
	"
options="!archcheck !check"

build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
	#install -Dm644 "$srcdir"/deviceinfo "$pkgdir"/usr/share/deviceinfo/deviceinfo
}

sha512sums="
0a1aa091e0d9039aa4c6624d9d595992c6875af5c99ff34216cd4fad5d634aee5698c722b4db7d8a52562e016f7a791a0e5fa4f228417c3276524b327611ab87  deviceinfo
e70bae17df23dcaaaea0e2d3616556f04baa23f8ee1357785c0f539bf97282d8ddff53953e155b72689bb73beb38c2da3d08de2a61e866684edfa10a6593885d  modules-initfs
"
