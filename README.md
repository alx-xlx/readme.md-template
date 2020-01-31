

<a href="https://colab.research.google.com/github/alx-xlx/Instagram-Metadata/blob/master/Instagram-Metadata.ipynb" target="_parent"><img style="display:block;margin-left:auto;margin-right:auto" src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

# readme.md-template
 Beautify you Readme.md File

[![GitHub issues](https://img.shields.io/github/issues/alx-xlx/readme.md-template)](https://github.com/alx-xlx/readme.md-template/issues)
[![GitHub forks](https://img.shields.io/github/forks/alx-xlx/readme.md-template)](https://github.com/alx-xlx/readme.md-template/network)
[![GitHub stars](https://img.shields.io/github/stars/alx-xlx/readme.md-template)](https://github.com/alx-xlx/readme.md-template/stargazers)
[![GitHub license](https://img.shields.io/github/license/alx-xlx/readme.md-template)](https://github.com/alx-xlx/readme.md-template/blob/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/url?label=Github&logo=github&style=social&url=http%3A%2F%2Fgithub.com%2Falx-xlx)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Falx-xlx%2Freadme.md-template)

![Discord](https://img.shields.io/discord/655868052860174357?label=Discord&logo=discord)

![GitHub commit activity](https://img.shields.io/github/commit-activity/w/alx-xlx/readme.md-template?label=Commit%20Activity) ![GitHub last commit](https://img.shields.io/github/last-commit/alx-xlx/readme.md-template?color=success&label=Last%20Commit) ![GitHub contributors](https://img.shields.io/github/contributors/alx-xlx/readme.md-template?label=Contributors) ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/alx-xlx/readme.md-template) ![GitHub repo size](https://img.shields.io/github/repo-size/alx-xlx/readme.md-template)

![Total Clone](https://img.shields.io/badge/dynamic/json?color=brightness&label=Total%20Cloned&query=count&url=https%3A%2F%2Fviralcourse.online%2Ftools%2Fgithub-clone-status%2Fclone-status.php) ![Unique Clone](https://img.shields.io/badge/dynamic/json?color=brightness&label=Unique%20Cloned&query=uniques&url=https%3A%2F%2Fviralcourse.online%2Ftools%2Fgithub-clone-status%2Fclone-status.php) ![Total Views](https://img.shields.io/badge/dynamic/json?color=brightness&label=Total%20Views&query=count&url=https%3A%2F%2Fviralcourse.online%2Ftools%2Fgithub-clone-status%2Fviews-status.php) ![Unique Views](https://img.shields.io/badge/dynamic/json?color=brightness&label=Unique%20Views&query=uniques&url=https%3A%2F%2Fviralcourse.online%2Ftools%2Fgithub-clone-status%2Fviews-status.php)

## Important Links

https://shields.io/category/build
https://github.com/BraveUX/for-the-badge


https://stackoverflow.com/questions/33999475/prevent-direct-url-access-to-php-file/33999539
https://stackoverflow.com/questions/356705/how-to-send-a-header-using-a-http-request-through-a-curl-call

---
https://stackoverflow.com/questions/1939609/convert-command-line-curl-to-php-curl
https://incarnate.github.io/curl-to-php/

```
curl -u USERNAME:PASSWORD -H 'Content-Type: application/json; charset=utf-8' -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.130 Safari/537.36' https://api.github.com/repos/alx-xlx/Instagram-Metadata/traffic/clones
```

OR

```
curl -u USERNAME:PASSWORD https://api.github.com/repos/alx-xlx/Instagram-Metadata/traffic/clones
```

PHP

`sudo apt-get install php-curl`

---
Run PHP cmds
https://www.php.net/manual/en/function.exec.php


[Traffic API](https://developer.github.com/v3/repos/traffic/)




----------

A. Make a new `traffic-status.php` file in your SECURE ONLINE SERVER

B. Replace the Variable in Below Code with yours

`USERNAME`, `REPOSITORY`, `GRAPH`

GRAPH  (Replace GRAPH with any one of the following) [Read Here](https://developer.github.com/v3/repos/traffic/)
1. `popular/referrers`
2. `popular/paths`
3. `views`                  
4. `clones`                


```
<?php
$url = 'https://api.github.com/repos/USERNAME/REPOSITORY/traffic/GRAPH';
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, $url);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, true);

curl_setopt($ch, CURLOPT_USERPWD, 'USERNAME' . ':' . 'PASSWORD');

$headers = array();
$headers[] = 'Content-Type: application/json; charset=utf-8';
$headers[] = 'User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.130 Safari/537.36';
curl_setopt($ch, CURLOPT_HTTPHEADER, $headers);
$response = curl_exec($ch);
curl_close($ch);
echo($response);
?>
```

C. Copy the edited code in your `traffic-status.php` file & save.

D. Now upon visiting the URL of your file you will get the `json` response

E. Goto [shields.io](https://shields.io/) & in the `Dynamic Section`
1. data type - json
2. label - your label (any)
3. data url - URL to your `traffic-status.php`
4. query - [Read Here](https://developer.github.com/v3/repos/traffic/) e.g `count`
5. color - green (any)
6. prefix - (leave blank)
7. suffix - (leave blank)

