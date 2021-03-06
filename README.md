
# How to downgrade or install a specific version of Composer?

Assuming a regular composer installation, to rollback to version 1 of composer, you simply execute:
```
composer self-update --1
```
When you want to go back to version 2 (which you should, after updating or removing the incompatible plugins):
```
composer self-update --2
```
The above will take you to the latest on any of the two major versions.

You can also "update" to a specific version just by passing the version number to self-update:
```
composer self-update 1.10.12
composer self-update 2.0.7

```
After performing any self-update, you can specify --rollback to go back to the previously installed version.
```
composer self-update
composer self-update --rollback

```
Finally, if you are feeling adventurous, you can update to a pre-release version by executing:
```
composer self-update --preview
```
