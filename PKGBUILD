# Author: Filirom1 <filirom1@gmail.com>
# Maintainer: Filirom1 <filirom1@gmail.com>
_npmname=stripcolorcodes
pkgname=nodejs-stripcolorcodes # All lowercase
pkgver=0.1.0
pkgrel=1
pkgdesc="Remove color codes (special characters) with nodejs"
arch=(any)
url="http://github.com/Filirom1/stripcolorcodes"
license=(MIT)
depends=('nodejs' )
optdepends=()
source=(http://registry.npmjs.org/$_npmname/-/$_npmname-$pkgver.tgz)
noextract=($_npmname-$pkgver.tgz)
sha1sums=(1e4ba1b9fef8cc2f0f705bda2bd99db3bca55c80)
build() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p $_npmdir
  cd $_npmdir
  npm install -g --prefix "$pkgdir/usr" $_npmname@$pkgver
}
# vim:set ts=2 sw=2 et: