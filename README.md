# moment-mini

Minified version of moment-library that only supports necessary locales.


## Create minified moment

1. Clone moment project
    ```shell
    git clone https://github.com/moment/moment.git
    ```
1. Change directory
    ```shell
    cd moment
    ```

1. Install dependencies
    ```shell
    npm install
    ```

1. Use Grunt task to compile Moment with a custom list of locales
    ```shell
    grunt transpile:fi,sv,en-gb
    ```

## Create moment-mini library

1. Copy generated moment file and paste it in the moment-mini directory

    ```shell
    cp .\moment\build\umd\min\moment-with-locales.custom.js .\moment-mini\
    ```

1. Create library

    ```shell
    npm pack
    ```

## Add library to your project

1. Install to your project

    ```shell
    npm install <moment-mini-path>\moment-<version>.tgz
    ```

## References

https://momentjs.com/docs/#/i18n/loading-into-browser/
