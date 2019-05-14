# Mandela
Development site setup

Add the following lines to the bottom of settings.php to show all errors

```
error_reporting(-1);
$conf['error_level'] = 2;
ini_set('display_errors', TRUE);
ini_set('display_startup_errors', TRUE);
```

In BASH shell:

```
sudo chmod +w sites/default/settings.php
tee -a sites/default/settings.php << END
error_reporting(-1);
$conf['error_level'] = 2;
ini_set('display_errors', TRUE);
ini_set('display_startup_errors', TRUE);
END
sudo chmod -w sites/default/settings.php
```
