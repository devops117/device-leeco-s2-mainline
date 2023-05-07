pkgname=device-leeco-s2-mainline
pkgdesc="LeEco Le 2"
pkgver=1.0
pkgrel=2
url="https://postmarketos.org"
license="MIT"
arch="aarch64"
options="!check !archcheck"
depends="postmarketos-base mkbootimg soc-qcom-msm8916 linux-postmarketos-qcom-msm8976"
makedepends="devicepkg-dev"
source="deviceinfo"
subpackages="
	$pkgname-nonfree-firmware:nonfree_firmware
"
build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
}

nonfree_firmware() {
	pkgdesc="Proprietary firmware"
	depends="linux-firmware-qcom firmware-leeco-s2-mainline"
	mkdir "$subpkgdir"
}


sha512sums="
5839219199464c8f6195f3a6c61b84d6f7cc176b36e1b545fc0791f994ea678ba40894402f30b0f272a41871a695471429147c5525fa5b2fc54bc4c3a41f347a  deviceinfo
"
