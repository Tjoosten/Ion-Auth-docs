Documentation Ion Auth
=========================

Ion Auth is a simple and lightweight authentication library for de CodeIgniter framework.
That is released under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)

### Installation

1. [Download the latset version](https://www.github.com/benedmunds/CodeIgniter-Ion-Auth/zippball/2)
2. Copy the files form this package to the correspoding folder in your application folder. Fro example, copy Ion_auth/config/ion_auth.php to system/application/config/ion_auth.php
3. Run the appropriate SQL file form the :sql directory.

### Default login

- Email: admin@admin.com
- Password: password

### Upgrading

1. [Download the latest version](https://github.com/benedmunds/Codeigniter-Ion-Auth/zipball/2)
2. Overwrite "libraries/ion_auth.php" and "models/ion_auth_model.php" with the new versions.

### Loading Ion Auth

You load Ion Auth. Just link any other library. Or you can also autoload the library.

```php
// Load into controller
$this->load->library(array('ion_auth');

// Autoload
$autoload['libraries'] = array('ion_auth');
```

### Configuration

Ion Auth is extremely configurable. The following configuration options are available:
To change configuration options simply edit the ion_auth array as needed in /ion_auth.php.

### Info about the configuration variables

- `$config['tables']['groups']` - The table name to use for the groups table. DEFAULT is 'groups'.
- `$config['tables']['users']` - The table name to use for the users table. DEFAULT is 'users'.
- `$config['tables']['users_groups']` - The table name to use for the users groups table. Default is 'users_groups'.
- `$config['tables']['login_attemps']` - The table name to use for login attemps table. DEFAULT is 'login_attempts'.

- `$config['site_title']` = The title of your site, used for email.
- `$config['admin_email']` = Your administrator email address. DEFAULT os 'admin@example.com'.
- `$config['default_group']` = Name of the default user group. DEFAULT is 'members'.
- `$config['admin_group']` = Name of the admin group. DEFAULT is 'admin'.
- `$config['join']['users']` = Users table colunm you want to join WITH. DEFAULT is 'user_id'. 
- `$config['join']['groups']` = Group table column you want to join WITH. DEFAULT is 'group_id'.

- `$config['identity']` = Column to use for uniquely identifing user/logging in/etc. Usual choices are 'email' OR 'username'. You should add an index in the users table for whatever you set this option to. DEFAULT is 'email'.

- `$config['min_password_length']` = Minimum length of passwords. DEFAULT is '8'.
