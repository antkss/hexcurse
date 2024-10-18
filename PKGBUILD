# Maintainer:  uffe < uffe at uffe dat org >
# Contributor: SpepS <dreamspepser at yahoo dot it>
# Contributor: eric <eric@archlinux.org>

pkgname=hexcurse
pkgver=1.60.0
pkgrel=1
pkgdesc="Versatile ncurses-based hex editor."
arch=('i686' 'x86_64')
url="https://github.com/LonnyGomes/hexcurse"
license=('GPL-2.0-only')
depends=('ncurses')
options=('!makeflags')

prepare() {
  echo "nothing"
}

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  ./configure --prefix=/usr --mandir=/usr/share/man

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make DESTDIR="${pkgdir}/" install
}

#
# EOF
#
