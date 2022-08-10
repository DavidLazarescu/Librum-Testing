# Librum

Librum's mission is to make your reading experience as <b>good</b> and <b>simple</b> as possible.

Librum offers lots of functionalities, which you can use through a <b>modern</b> and <b>simplistic</b> interface.<br>
With Librum, you can create and manage your own library of books and files, which you can access from <b>all</b> of your devices.<br>
You can comfortably read your book through the app, <b>highlight</b> sections you find interesting and add <b>bookmarks</b> on pages you want to revisit. On top, Librum
makes it possible for you, to take <b>notes</b> on what you've read, directly from the app.<br>
Librum also offers a <b>free</b> in-app bookstore, plugins to make you even more productive and the possibility, to fully customize the application, so that it looks and behaves as you want.

Librum's focus lies on being <b>modern</b>, completely <b>opensource</b>, <b>free</b> and <b>fast</b>.</br>
Everyone can download, modify and redistribute the source-code since we are using a complete copyleft license.

<br>

# Details

You will be able to use Librum across all major platforms, including:
- Windows
- GNU/Linux
- MacOS
- IOS
- Android

<br>

All common formats will be supported by Librum, this includes:
- Pdf
- Epub
- Mobi
- Txt
- Html
- ... and much more


<br><br>

# Getting started

Instructions to get Librum up and running in your environment.

<br>

## For GNU/Linux
### Prerequisites
- cmake (at least version 3.20)     https://cmake.org/download/
- make (or any other build system)  http://ftp.gnu.org/gnu/make/
- Qt6                               https://www.qt.io/download
- Gcc (or any other c++ compiler)   https://gcc.gnu.org/

### Installation
1. Clone the repository.
    ```sh
    git clone https://github.com/Etovex/Librum.git
    ```
2. Step into the cloned project folder.
    ```sh
    cd Librum
    ```
3. Add the Qt path to the CMakeLists.txt<br>
    By default, Qt creator appends the path to Qt to the 'CMAKE_PREFIX_PATH' variable, you have 2 options for building Librum:
    <br>
    - Use Qt Creator to build the project (Simply open the CMakeLists.txt through Qt Creator, by clicking File -> Open File or Project...)
    - Add the path manually, for that, just copy this line
        ```sh
        list(APPEND CMAKE_PREFIX_PATH "/home/<username>/Qt/<Version>/<compiler>")
        ```
        to the third line of the top-level CMakeLists.txt and replace all contents in angular brackets '<>' with your data, for example:
        ```sh
        list(APPEND CMAKE_PREFIX_PATH "/home/david/Qt/6.2.3/gcc_64")
        ```
4. Create the build folder and step into it.
    ```sh
    mkdir build-Release
    cd build-Release
    ```
6. Run cmake.
    ```sh
    cmake -DCMAKE_BUILD_TYPE:STRING=Release -DBUILD_TESTS=Off ..
    ```
    If you don't want to use your default build-file generator (e.g. make, or ninja), add the -G option, e.g.
    ```sh
    -G "Ninja"
    ```
    

6. Build the project
    ```sh
    make
    ```
7. Run the app
    ```sh
    ./appLibrum
    ```
<br>


<br>

## For Windows
### Prerequisites
- cmake (at least 3.20)            https://cmake.org/download/
- make (or any other build system) http://ftp.gnu.org/gnu/make/
- Qt6                              https://www.qt.io/download
- mingw                            https://sourceforge.net/projects/mingw/
### Installation
1. Clone the repository.
    ```sh
    git clone https://github.com/Etovex/Librum.git
    ```
2. Open the project in Qt creator by clicking on File -> Open File or Project... and selecting the CMakeLists.txt)
3. Run Librum
<br>

<br>

## For macOS
Not yet officially supported. Support coming soon!
