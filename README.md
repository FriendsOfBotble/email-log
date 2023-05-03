# Email Log for Botble CMS

Email Log for Botble CMS allows you to log all emails sent from the system. You can view envelope, headers, and body of the email, as well as the response from the SMTP server.

![Screenshot](art/screenshot.png)

## Installation

### Install via Marketplace

- Go to **Admin Panel** -> **Plugins** -> **Add New**, find the plugin and click **Install Now** button.

### Install from source

- Download the package from [Botble Marketplace](https://marketplace.botble.com/products/datlechin/email-log).
- Extract package to your plugins folder (`platform/plugins`).

### Usage

Go to **Admin Panel** -> **Plugins** -> **Email Log** and press **Activate** button.

All emails sent from the system will be logged automatically, you can view the log by clicking on the **Email Logs** menu item.

You can customize how many days you want to keep the email log by updating the `Keep email log for days` setting in **General Settings**.

![Admin settings](art/settings.png)

Then you can run the command to delete old email logs:

```bash
php artisan model:prune --model="Datlechin\EmailLog\Models\EmailLog"
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email datlechin@gmail.com instead of using the issue tracker.

## Credits

-   [Ngo Quoc Dat](https://github.com/datlechin)
-   [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
