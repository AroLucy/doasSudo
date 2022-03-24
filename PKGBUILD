pkgname=sudo
pkgver=1.9.10
pkgrel=1
pkgdesc="Trick packages that require sudo to use doas"
arch=('any')

source=("./$pkgname-$pkgver")
md5sums=("86e3e82004c8fcba86c84dd5c6bdeb1e")

depends=(
	'python'
	'doas'
)
conflicts=('sudo')
provides=(
	'sudo'
)

package() {
	install -Dm644 "sudo-$pkgver" "$pkgdir/usr/bin/sudo"
	install -Dm644 "sudo-$pkgver" "$pkgdir/usr/lib/sudo"
	chmod a+x "$pkgdir/usr/bin/sudo"
	chmod a+x "$pkgdir/usr/lib/sudo"
}
