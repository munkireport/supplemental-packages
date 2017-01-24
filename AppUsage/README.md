# AppUsage

These packages are needed to supply the [App Usage](https://github.com/munkireport/munkireport-php/tree/master/app/modules/appusage/README.md) module with data. These steps only need to be taken once.

1. Download this repo: [click here](https://github.com/munkireport/supplemental-packages/archive/master.zip)
1. Unzip the Download
1. Use `munkiimport` to import 'crankd' and the 'crankd_application_usage' package making them an 'update_for' your Munkireport package.

  **Note**: If your Munkireport package is named differently please modify the `--update_for` flag accordingly.

    ```bash
    $ munkiimport ~/Downloads/supplemental-packages-master/AppUsage/crankd.pkg --update_for="Munkireport" --unattended_install
    ```

    ```bash
    munkiimport ~/Downloads/supplemental-packages-master/AppUsage/crankd_application_usage.pkg --update_for="Munkireport" --unattended_install
    ```


# Resources

If you wish to build these packages yourself you can utilize [munkipkg](https://github.com/munki/munki-pkg) plus the [github.com/munki/munki-pkg-projects](https://github.com/munki/munki-pkg-projects) repo.

Source files:
* crankd - [https://github.com/munki/munki-pkg-projects/tree/master/crankd](https://github.com/munki/munki-pkg-projects/tree/master/crankd)
* application_usage source files - [https://github.com/google/macops/tree/master/crankd](https://github.com/google/macops/tree/master/crankd)
