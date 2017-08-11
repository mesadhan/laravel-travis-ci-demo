<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
</p>

## About This Repository

The purpose of this repository is to have a ready-to-develop Laravel installation with documented workflow of a new project start. **One size does not fit all**

## Workflow

@todo

## Troubleshooting

We will attempt to cover the most common issues that we encounter. If it is not listed here - feel free to make a pull-request with your issue solution!

### Error `Facebook\WebDriver\Exception\WebDriverCurlException: Curl error thrown for http POST to /session with params:` solving:

Open new terminal window, launch these commands:

```bash
sudo apt-get update
sudo apt-get -y install libxpm4 libxrender1 libgtk2.0-0 libnss3 libgconf-2-4
sudo apt-get -y install chromium-browser
sudo apt-get -y install xvfb gtk2-engines-pixbuf
sudo apt-get -y install xfonts-cyrillic xfonts-100dpi xfonts-75dpi xfonts-base xfonts-scalable
sudo apt-get -y install imagemagick x11-apps
chmod a+x ./vendor/laravel/dusk/bin/chromedriver-linux
Xvfb :0 -screen 0 1280x960x24 &
```

After you have launched them, open your main window and run dusk tests. It should be up and running.

If you encounter more issues with this error, visit: [Github issue page](https://github.com/laravel/dusk/issues/50)

## Contributing

Everyone is welcome to contribute to this repository as long as it helps the community.

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell at taylor@laravel.com. All security vulnerabilities will be promptly addressed.

We have not modified/changed the core/code more than adding few packages that we trust. If you don't trust them - feel free to remove.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).
