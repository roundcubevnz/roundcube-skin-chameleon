Chameleon Kolab Enterprise Roundcube Skin
================================

Rounducube skin in sync from [Chameleon](https://git.kolab.org/diffusion/RSC/), 
also known as Kolab Enterprise Web Client Skin.


![Kolab Theme](screenshots/roundcubemail-skin-chameleon-1.jpg)

## installation

Just copy it content **as `chameleon` directory** into your Roundcube instance/skins directory.

**Chameleon depends on Larry, so this skin must be installed too.**

## Hacking

styles.css is written using LESS syntax, compiled with `lessc` by `nodejs-less`
but there's better options like https://github.com/codeigniterpower/compiler-lessphp

 $ lessc -x styles.less > styles.css

(the -x option minifies the CSS code)

References to image files from the included CSS files can be appended
with cache-buster marks to avoid browser caching issues after updating.

Run `bin/updatecss.sh --dir <path-to-chameleon-skin>` from the Roundcube
package before packaging the skin or after installing it on the
destination system.

# License
Screendesign and icons by [Kolab Systems AG, Zurich, Switzerland](http://kolabsys.com)

The contents of this folder can be redistributed and/or modified
under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, either version 3 of the License,
or (at your option) any later version.


