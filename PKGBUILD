pkgname=pdfjs-legacy
pkgver=5.4.149
pkgrel=1
pkgdesc="PDF reader in javascript - legacy distribution"
conflicts=(pdfjs)
arch=('x86_64')
url="https://mozilla.github.io/pdf.js/"
license=('Apache-2.0')
source=("https://github.com/mozilla/pdf.js/releases/download/v${pkgver}/pdfjs-${pkgver}-legacy-dist.zip")
sha256sums=('048b6badace8d4b3a389aeb51c3733a2ae76ded764760f755254797141f7c05b')

package() {
  mkdir -p "$pkgdir/usr/share/pdf.js"
  cp -R "$srcdir"/{LICENSE,build,web} "$pkgdir/usr/share/pdf.js"
  find "$pkgdir" -type f -exec chmod 644 {} \;  
}
