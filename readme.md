# Curriculum Vitae of Davide Franchinetti

This repository hosts my CV in Italian and English (updated 5 May 2022).

It includes the PDF output so you can download and view it directly even if you don't want to compile it yourself with LaTeX.

---

## Important Notes

As mentioned in the comments at the beginning of the `.tex` files, the CV is based on the [Plasmati CV template by Alessandro Plasmati](https://www.latextemplates.com/template/plasmati-cv). In order to make the template work you must compile it with `XeLaTeX`, using the [Fontin font by exljbris Font Foundry](https://www.exljbris.com/fontin.html).

For some reason, with the TeXLive distribution and Fontin installed on my main PC using Windows 10, **XeLaTeX couldn't find the font and I kept getting compilation errors**. Because of that, I had to manually copy the `.otf` font files inside the TeXLive public font directory. To find your TeXLive installation directory you can execute the following command:
```
$ tlmgr version

tlmgr revision 63033 (2022-04-15 07:19:42 +0200)
tlmgr using installation: C:/texlive/2022
TeX Live (https://tug.org/texlive) version 2022
```

Once the installation directory is located, the right path for placing the `.otf` files in my case was:
```
<tex directory>\texmf-dist\fonts\opentype\public\fontin
```
Be aware that with a different LaTeX distribution and/or operating system the path might be different as well. After that I executed:
```
$ fc-cache -fsv
```
Theoretically it's a Linux command, but it works even in `Powershell`. Maybe it wasn't necessary in this case or there's some other kind of fix for the issue above. If you know more, feel free to report it here.

---

## Acknowledgments

Many thanks to Simone Robutti ([chobeat](https://github.com/chobeat)) and Michelangelo Carocci for inspiration and support.

---

## License
[CC BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)
