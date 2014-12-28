Documentation Ion Auth
=========================

Ion Auth is a simple and lightweight authentication library for de CodeIgniter framework.
That is released under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)

### Installation

1) [Download the latset version](https://www.github.com/benedmunds/CodeIgniter-Ion-Auth/zippball/2)
2) Copy the files form this package to the correspoding folder in your application folder. Fro example, copy Ion_auth/config/ion_auth.php to system/application/config/ion_auth.php
3) Run the appropriate SQL file form the :sql directory.

### Default login

- Email: admin@admin.com
- Password: password

### Upgrading

1) [Download the latest version](https://github.com/benedmunds/Codeigniter-Ion-Auth/zipball/2)
2) Overwrite "libraries/ion_auth.php" and "models/ion_auth_model.php" with the new versions.

### Loading Ion Auth

You load Ion Auth. Just link any other library. Or you can also autoload the library.

```php
// Load into controller
$this->load->library(array('ion_auth');

// Autoload
$autoload['libraries'] = array('ion_auth');
```

### Configuration options

Ion Auth is extremely configurable. The following configuration options are available:

```php
$config['tables']['groups']
$config['tables']['users']
$config['tables']['users_groups']
$config['tables']['login_attemps']
$config['site_title']
$config['admin_email']
$config['default_group']
$config['admin_group']
$config['join']['users']
$config['join']['groups']
$config['identity']
$config['min_password_length']
$config['max_password_length']
$config['email_activation']
$config['remember_users']
$config['user_expire']
$config['user_extend_on_login']
$config['email_type']
$config['email_templates']
$config['email_activate']
$config['email_forgot_password']
$config['email_forgot_password_complete'] 
$config['salt_length']
$config['store_salt']
$config['forgot_password_expiration']
$config['track_login_attempts']
$config['maximum_login_attempts']
$config['message_start_delimiter']
$config['message_end_delimeter']
$config['error_start_delimiter']
$config['error_end_delimeter']
```

### Using the config file

To change configuration options simply edit the ion_auth array as needed in /ion_auth.php.

`tables['groups']` - The table name to use for the groups table. DEFAULT is 'groups'.
`tables['users']` - The table name to use for the users table. DEFAULT is 'users'.
`tables['users_groups']` - The table name to use for the users groups table. Default is 'users_groups'.
