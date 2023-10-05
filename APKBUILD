pkgname=device-leeco-s2-mainline
pkgdesc="LeEco Le 2"
pkgver=1.0
pkgrel=1
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
363470dae416bf528e96b4880c3506c66162fd9be8754cae1120b43fbe33efa830e8dbb2c6541ca208e03a607496fd4e05c36150d2a47c9de4fc4631a25cf800  deviceinfo
"
