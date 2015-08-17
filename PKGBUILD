# Maintainer: Patrice Peterson <runiq at archlinux dot us>
# Contributor: JonnyJD <arch@JonnyJD.net>

pkgname=python-secretstorage
pkgver=2.1.1
pkgrel=1
pkgdesc="Securely store passwords and other private data using the SecretService DBus API"
arch=('any')
url="https://pypi.python.org/pypi/SecretStorage"
license=('BSD')
depends=('python-dbus'
         'python-crypto')
source=("$pkgname-$pkgver.tar.gz"::https://pypi.python.org/packages/source/S/SecretStorage/SecretStorage-${pkgver}.tar.gz)
md5sums=('0c5c875104ebb6f6d45c7faf6c2943f9')

package() {
  cd SecretStorage-$pkgver
  python setup.py install --root="$pkgdir"
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
