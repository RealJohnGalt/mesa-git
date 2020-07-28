# Maintainer: Lone_Wolf <lone_wolf@klaas-de-kat.nl>
# Contributor: Armin K. <krejzi at email dot com>
# Contributor: Kristian Klausen <klausenbusk@hotmail.com>
# Contributor: Egon Ashrafinia <e.ashrafinia@gmail.com>
# Contributor: Tavian Barnes <tavianator@gmail.com>
# Contributor: Jan de Groot <jgc@archlinux.org>
# Contributor: Andreas Radke <andyrtr@archlinux.org>
# Contributor: Thomas Dziedzic < gostrc at gmail >
# Contributor: Antti "Tera" Oja <antti.bofh@gmail.com>
# Contributor: Diego Jose <diegoxter1006@gmail.com>

pkgname=mesa-git
pkgdesc="an open-source implementation of the OpenGL specification, git version"
pkgver=20.2.0_devel.126589.1882b1e5a7d
pkgrel=1
arch=('x86_64')
makedepends=('git' 'python-mako' 'xorgproto'
              'libxml2' 'libx11'  'libvdpau' 'libva' 'elfutils' 'libomxil-bellagio' 'libxrandr'
              'ocl-icd' 'libgcrypt'  'wayland' 'wayland-protocols' 'meson' 'ninja')
depends=('libdrm' 'libxxf86vm' 'libxdamage' 'libxshmfence' 'libelf'
         'libomxil-bellagio' 'libunwind' 'libglvnd' 'wayland' 'lm_sensors' 'libclc' 'glslang' 'vulkan-icd-loader' 'zstd')
optdepends=('opengl-man-pages: for the OpenGL API man pages')
provides=('mesa' 'opencl-mesa' 'vulkan-intel' 'vulkan-radeon' 'vulkan-mesa-layer' 'libva-mesa-driver' 'mesa-vdpau' 'vulkan-driver' 'opengl-driver' 'opencl-driver')
conflicts=('mesa' 'opencl-mesa' 'vulkan-intel' 'vulkan-radeon' 'vulkan-mesa-layer' 'libva-mesa-driver' 'mesa-vdpau')
url="https://www.mesa3d.org"
license=('custom')
source=('mesa::git+https://gitlab.freedesktop.org/mesa/mesa.git'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5924.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5980.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5968.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5750.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5728.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5966.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/6063.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/6063.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/6072.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/6073.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/6074.diff'
                'https://gitlab.freedesktop.org/pepp/mesa/-/commit/d71ff5b42cab85817e5c22c5e21eeaca87e39dec.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/commit/d4d6d1557d03ac7db054798bdd9de683c1622e71.diff'
                'LICENSE')
md5sums=('SKIP'
         'd16332b2811550208a64e768aa9701c7'
         'a4a374ff049778f0b8c4666ee6f7ad20'
         '7964d9537e1927babb95eb2383dbf520'
         '560ebaec0715b95010590f952b918989'
         'f5790c785525365eb9a46fe48812c6aa'
         '1a159646705332e0eae0968b15b9a416'
         'cfce5e45e07e4f15816ec514e0b867e5'
         'cfce5e45e07e4f15816ec514e0b867e5'
         'fe5a7d188a0b9a52e4312c34022c869b'
         'c7951c927603dc25c69e80b2f097c892'
         'c00ac7053c647b08d471db523781bbb5'
         'd92c6a427f007f563516f01f84358283'
         '790e23e85b78ba05330587cf4663401d'
         '5c65a0fe315dd347e09b1f2826a1df5a')
sha512sums=('SKIP'
            '79dbe9d4c5f24a97acb1d445bf47d9dd351ca61036e0d6ffdba3e51ac736699afb6bae7a1d327776690ae3261acd520dd0fde171b4b2f991f0a2063398bfc3c7'
            'cc9770cd7828821eb7f13347747fb452fa2e0f1b97bbeb4e8ec3085dbba92292da12c8b41fc2cf41206dff5bfc04247ca031813af3dc233a17b5e7b27cdf0b54'
            '40b904e951099a5bdd4d449e7a7063762ed4e8d957332bdf1baab53b594a6b4bc3040ab47c02aeb448a8eec9641b7d7e8633e2bcb443e52a1afe36fa49ba4289'
            '2e59abb5c4bf51e363ce73f166287411f971d9dd146f57a133524e67b37e3656baaf21a8f9f5fc2b07fca271d7bea9d15110a8f430e84ab0009251cc653fb081'
            '889565e9a5cc4b1564fab1156b0a88b77e9802d56a5792b315d2552812c4eb478682b9f7046b89c0e41cd2492f768bd009ec2d5bf570fb42345910c4fe0d28b4'
            'c6970e37160009dbff04fa066c7789ec9372ada82534a1df51ec8596dbca71940f72655a46940ba3ce5dba1ed34362ac26cd31f8d762167ed269b40eea2d74d5'
            '43cd3a78712a39d39ec343f537620f271c7741a55424cc37e211a36a661df5c5481049754695431de81694a64077d3467fc08b90dafa7cd33581f879bc502fea'
            '43cd3a78712a39d39ec343f537620f271c7741a55424cc37e211a36a661df5c5481049754695431de81694a64077d3467fc08b90dafa7cd33581f879bc502fea'
            'ff09a1b35c9473013e560a486394cf04676f0c2cd743f50365aa5adfd08ffe253c558291f925a23c8e9e1406e909ed5ca091703b597819b62a714f047a10edbe'
            'd5475b65b839cdb85860351f0c54609769a5465143dcd0d05901452fb307220bff3584ee6d19957dd3aa82dd29d6908e3d6f637c0d5c68fa5fcae8225a8f2cf9'
            'c54c3ef148bb52f3788586c1fa4c739be6f3b779a1e722fde58e4a64938465f0ac978e4f0c962cbae0efc90f5304ca1853385162d2ce7a29d931cbf76acc7ac8'
            '37e3630ce56d003044168f25c54f65d84e78df386a5405fd1936a3754e85125c64db7fb235d202d578ee8b7e4c736a86632658eb2badb54ac7602d0f248e2783'
            '3610ff9aa85b55ce9b86367401464f93562953807fe11cee09617832dae215e49b37072487324b0b50aa940a3a27e59bf4087d8b75e531b815aec0b629911cad'
            '25da77914dded10c1f432ebcbf29941124138824ceecaf1367b3deedafaecabc082d463abcfa3d15abff59f177491472b505bcb5ba0c4a51bb6b93b4721a23c2')

# NINJAFLAGS is an env var used to pass commandline options to ninja
# NOTE: It's your responbility to validate the value of $NINJAFLAGS. If unsure, don't set it.

# MESA_WHICH_LLVM is an environment variable that determines which llvm package tree is used to built mesa-git against.
# Adding a line to ~/.bashrc  that sets this value is the simplest way to ensure a specific choice.
#
# NOTE: Aur helpers don't handle this method well, check the sticky comments on mesa-git aur page .
#
# 1: llvm-minimal-git (aur) preferred value
# 2: AUR llvm-git
# 3: llvm-git from LordHeavy unofficial repo 
# 4  llvm (stable from extra) Default value
# 

if [[ ! $MESA_WHICH_LLVM ]] ; then
    MESA_WHICH_LLVM=4
fi

case $MESA_WHICH_LLVM in
    1)
        # aur llvm-minimal-git
        makedepends+=('llvm-minimal-git')
        depends+=('llvm-libs-minimal-git')
        optdepends+=('llvm-minimal-git: opencl')
        ;;
    2)
        # aur llvm-git
        # depending on aur-llvm-* to avoid mixup with LH llvm-git
        makedepends+=('aur-llvm-git')
        depends+=('aur-llvm-libs-git')
        optdepends+=('llvm-git: opencl')
        ;;
    3)
        # mesa-git/llvm-git (lordheavy unofficial repo)
        makedepends+=('llvm-git' 'clang-git')
        depends+=('llvm-libs-git')
        optdepends+=('clang-git: opencl' 'compiler-rt: opencl')
        ;;
    4)
        # extra/llvm
        makedepends+=(llvm=10.0.0 clang=10.0.0)
        depends+=(llvm-libs=10.0.0)
        optdepends+=('clang: opencl' 'compiler-rt: opencl')
        ;;
    *)
esac
        
        
        
        
        
pkgver() {
    cd mesa
    read -r _ver <VERSION
    echo ${_ver/-/_}.$(git rev-list --count HEAD).$(git rev-parse --short HEAD)
}

prepare() {
    # although removing _build folder in build() function feels more natural,
    # that interferes with the spirit of makepkg --noextract
    if [  -d _build ]; then
        rm -rf _build
    fi
    cd "${srcdir}/mesa"
    patch -p1 < "${srcdir}/5924.diff"
    #patch -p1 < "${srcdir}/5980.diff"
    patch -p1 < "${srcdir}/5968.diff"
    patch -p1 < "${srcdir}/5750.diff"
    patch -p1 < "${srcdir}/5966.diff"
    patch -p1 < "${srcdir}/6063.diff"
    patch -p1 < "${srcdir}/6072.diff"
    patch -p1 < "${srcdir}/6073.diff"
    patch -p1 < "${srcdir}/6074.diff"
    patch -p1 < "${srcdir}/d71ff5b42cab85817e5c22c5e21eeaca87e39dec.diff"
    patch -p1 < "${srcdir}/d4d6d1557d03ac7db054798bdd9de683c1622e71.diff"
    patch -p1 -R < "${srcdir}/5728.diff"

}

build () {
    meson setup mesa _build \
       -D b_ndebug=true \
       -D b_lto=false \
       -D buildtype=plain \
       --wrap-mode=nofallback \
       -D prefix=/usr \
       -D sysconfdir=/etc \
       -D platforms=x11,wayland,drm,surfaceless \
       -D dri-drivers=i915,i965,r200,r100,nouveau \
       -D gallium-drivers=r300,r600,radeonsi,nouveau,svga,swrast,virgl,iris,zink \
       -D vulkan-drivers=amd,intel \
       -D dri3=enabled \
       -D egl=enabled \
       -D gallium-extra-hud=true \
       -D gallium-nine=true \
       -D gallium-omx=bellagio \
       -D gallium-va=enabled \
       -D gallium-vdpau=enabled \
       -D gallium-xa=enabled \
       -D gallium-xvmc=disabled \
       -D gbm=enabled \
       -D gles1=disabled \
       -D gles2=enabled \
       -D glvnd=true \
       -D glx=dri \
       -D libunwind=enabled \
       -D llvm=enabled \
       -D lmsensors=enabled \
       -D osmesa=gallium \
       -D shared-glapi=enabled \
       -D gallium-opencl=icd \
       -D valgrind=disabled \
       -D vulkan-overlay-layer=true \
       -D vulkan-device-select-layer=true \
       -D tools=[] \
       -D zstd=enabled \
       
    meson configure _build
    
    # quoted from https://www.mesa3d.org/meson.html
    # Note: autotools automatically updated translation files (used by the DRI configuration tool) as part of the build process, Meson does not do this. 
    # Instead, you will need do this: 
    # ninja $NINJAFLAGS -C _build xmlpool-pot xmlpool-update-po xmlpool-gmo
    # mesa devs handle driconf translation differently now, above command is no longer needed
    ninja $NINJAFLAGS -C _build
}

package() {
    DESTDIR="${pkgdir}" ninja $NINJAFLAGS -C _build install

    # remove script file from /usr/bin
    # https://gitlab.freedesktop.org/mesa/mesa/issues/2230
    rm "${pkgdir}/usr/bin/mesa-overlay-control.py"
    rmdir "${pkgdir}/usr/bin"
    
    # indirect rendering
    ln -s /usr/lib/libGLX_mesa.so.0 "${pkgdir}/usr/lib/libGLX_indirect.so.0"
  
    install -Dt "${pkgdir}/usr/share/licenses/${pkgname}" "${srcdir}/LICENSE"
}
