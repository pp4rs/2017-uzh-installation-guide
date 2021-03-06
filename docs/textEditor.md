# Text Editors

A good text editor lies at the heart of any serious programmer's toolkit: It can do almost anything and makes you much more productive. The editors built into each program are generally are not an option (we will find certain cases where you may want to use them).

!!! danger "Updated for 2017"
    This year we are encouraging all participants to use the text editor [Atom](https://atom.io/).
    We hope this helps smooth out differences between text editors.

Please download, install it along with the necessary packages and stick with it for at least the duration of the course and assignment to get a feel for how it works.
There is a slight learning curve, but soon you hopefully be wondering why no-one forced you to do this before!
We should get you past the steepest part of the learning curve during the course itself, so we don't anticipate you struggling on your own.

!!! note
    None of the skills we learn in the course are tied to Atom, so if you do decide to move away to another editor, nothing will be lost.

<!-- ## Installing Sublime Text

Go to the [downloads page](https://www.sublimetext.com/3) and download the live installer for your operating system. -->

## Installing Atom

### Mac and Windows Users

Go to the [downloads page](https://github.com/atom/atom/releases/tag/v1.9.9) and download the live installer for your operating system.


### Linux/Ubuntu users

Enter the following information to add a repository that has the Atom installation, then press `Return`:

```bash
sudo add-apt-repository ppa:webupd8team/atom
```

Install Atom by entering the following commands into a terminal and then pressing `Return:`

```bash
sudo apt update; sudo apt install atom
```

## Verifying Atom Installation for Linux and Mac

We want Atom to be available from the command line. For Mac and Linux Users this is the default so if you type the following into the command line:

```bash
atom --version
```
followed by pressing `Return` you should see output like the following
```bash
Atom    : 1.12.7
Electron: 1.3.13
Chrome  : 52.0.2743.82
Node    : 6.5.0
```
Make sure that the version numbers are equal to whats above or newer.

!!! danger "Additional Step for Windows:"
    Getting things to run from the command line for us is a bit harder. You will need local administration rights for your computer, but you should have these on your personal computers or those owned by the Department.

    Right-click on Computer. Then go to "Properties" and select the tab "Advanced System Settings". Choose "Environment Variables" and select `Path` from the list of system variables.

    If you accepted all defaults during your installation, and didn't have any other non-default setting prior to starting this guide, choose `Edit.`

    **On Windows 7 or 8 machines:**
     Append the following (i.e., do not overwrite the previous value) modifying the string, with your relevant `username`:

            ;C:\Users\username\AppData\Local\atom\bin

    to the variable value – make sure the rest remains as it is and do not include spaces between the ";" and preceeding text.

    **On Windows 10 machines:**
    Click `New` and paste the following string, modifying the `username`

            C:\Users\username\AppData\Local\atom\bin

    Click on `OK` as often as needed.

    Close your current terminal session, open a new one, and again try `atom .` - the Atom editor will open if this was successful.

## Additional Packages for Atom

One of the advantages of Atom is that there are many *packages* that make your life easier, ranging from simple syntax highlighting to environments that can mimic a complete graphical user interface.

For this course, we will install the minimum number of packages necessary to make your coding life easier.

## Installing Additional Packages for Atom

Atom's package manager is built in to the program itself and is relatively easy to interact with.
To access Atom's settings press `Ctrl + ,` on your keyboard then click on the `Install` tab which is visible on the left hand side.

On the Installation page there is a prompt where you can type in a package name and then press `Return` and Atom will search for that package for you and return results with similar names.
When you find the package that you need, you click the blue 'Install' button and the package will be installed.

For this course, please install the following packages:

*   autocomplete-r
*   autocomplete-python
*   autoflow
*   language-sql
*   language-r
*   linter
*   linter-python
*   linter-lintr
*   tablr

If during the installation of a package Atom asks to install dependencies, always choose to accept.

!!! tip
    If you decide to stick with Atom after this course, you may find the following packages useful in your day to day work:

    *   language-latex
    *   language-markdown
    *   language-matlab
    *   language-stata
    *   markdown-writer
    *   markdown-preview-plus
    *   whitespace

    Feel free to ask us for whatever other packages we use to make our programming lives easier during some downtime.

<!-- ## Additional Package for Sublime Text

For those who want to use Sublime Text as their editor, you will need to add an additional package, "Package Control" to it so that we can customize it a little throughout the course. Proceed as follows:

Open the Sublime Text console via the using the ctrl+` shortcut or the View > Show Console menu.
Once open, paste the code below into the console (and press return):

        import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

We will show you how to use Package Control during the course. -->
