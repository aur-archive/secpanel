# Maintainer: enderst <enderst@gmail.com>
# Contributor: enderst <enderst@gmail.com>
pkgname=secpanel
pkgver=0.6.1
pkgrel=4
pkgdesc="Graphical frontend for managing and running SSH and SCP connections"
arch=('i686' 'x86_64')
url="http://themediahost.de/secpanel"
license=('GPL')
depends=('openssh' 'tcl' 'tk')
source=(http://downloads.sourceforge.net/project/$pkgname/$pkgname-$pkgver.tgz)
md5sums=('c94e598bc66d38421333b74a28abaa17')

package() {
	mkdir -p $pkgdir/usr/{bin,lib}
	cp -r $srcdir/usr/local/lib/secpanel $pkgdir/usr/lib/
	install -D -m755 $srcdir/usr/local/bin/secpanel $pkgdir/usr/bin/secpanel
}
