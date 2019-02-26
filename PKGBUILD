# Maintainer: Massimiliano Torromeo <massimiliano.torromeo@gmail.com>

pkgname=unyaffs
pkgver=0.9.7
pkgrel=2
pkgdesc="A program to extract files from a yaffs image"
arch=("i686" "x86_64")
url="https://git.bernhard-ehlers.de/ehlers/unyaffs"
license=(GPL)
depends=('glibc')

source=(https://git.bernhard-ehlers.de/ehlers/unyaffs/archive/0.9.7.tar.gz)
sha256sums=('17489fb07051d228ede6ed35c9138e25f81085492804104a8f52c51a1bd6750d')


build() {
	cd $pkgname
	make unyaffs
}

package() {
	cd $pkgname
	install -D -m 0755 unyaffs "$pkgdir"/usr/bin/unyaffs
}
