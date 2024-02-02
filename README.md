# Memulai Aplikasi-ci4
Memulai Aplikasi Codeigniter 4

1. Install Composer
2. Install Git Bash
3. Git bash here in the directory where the app will install
4. run command (mode install via composer)

```
$ composer create-project codeigniter4/appstarter nama_project project-root
```
replace *nama_project* with the real project name

or

```
$ composer create-project codeigniter4/appstarter nama_project --no-dev
```

if found errors

```
Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - codeigniter4/framework[4.0.0, ..., v4.4.5] require ext-intl * -> it is missing from your system. Install or enable PHP's intl extension.
    - Root composer.json requires codeigniter4/framework ^4.0 -> satisfiable by codeigniter4/framework[4.0.0, ..., v4.4.5].

To enable extensions, verify that they are enabled in your .ini files:
    - G:\xampp-7_4_30\php\php.ini
You can also run `php --ini` in a terminal to see which files are used by PHP in CLI mode.
Alternatively, you can run Composer with `--ignore-platform-req=ext-intl` to temporarily ignore these required extensions.
Running update with --no-dev does not mean require-dev is ignored, it just means the packages will not be installed. If dev requirements are blocking the update you have to resolve those problems.

```

Solution:
1. Open [xampp_folder_path]/php/php.ini to edit.
2. Search for ;extension=intl and remove the ;.
3. Save the php.ini file and restart Apache.
4. go to the htdocs folder and remove the current error project that have been made
5. got to git bash and run the above command again

# Install MPDF
```
$ composer require mpdf/mpdf
```

run the command inside the directory where the ci4 app installed

