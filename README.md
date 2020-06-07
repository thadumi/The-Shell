# The Shell

Minimalistic dark color theme for [Ghost](http://github.com/tryghost/ghost/) platform. Based on [The Shell](https://github.com/mityalebedev/The-Shell)

![image](https://user-images.githubusercontent.com/1761114/55421430-dc7f8e80-5581-11e9-9db8-ad3071f09098.png)

Live here: [https://thadumi.com](https://thadumi.com/).


# Enable the search bar

- Go into Ghost's admin panel > Settings > Integrations
- Create a custom integration named `ghostHunter`
- Intert the `Content API Key` into the following script
    ```html
        <script>
                var ghosthunter_key = 'INSERT_KEY_HERE';
                //optional: set your custom ghost_root url, default is "/ghost/api/v2"
                var ghost_root_url = '/ghost/api/v2';
        </script>
    ```
- Insert the updated script into Settings > Code Injection > Site Header

# Enable the Tags section
- Create a new page called Tags
- Page's Settings > Template and seletect `Tags`  
- Publish the page without adding content to it


# Run and Debug

Before running this theme locally you need to install Ghost.
```sh
sudo pacman -S nodejs-lts-erbium npm # Ghost requres node 10 or 12
sudo npm install --global gulp-cli

mkdir -p ghost-local && cd $_ && ghost install local
```

```sh
git clone https://github.com/thadumi/ghost-shell-theme.git

cd ghost-shell-theme

npm install
gulp watch
```

# Dependencies
- [ghostHunter](https://github.com/jamalneufeld/ghostHunter) for the search bar
- [nprogress](https://github.com/rstacruz/nprogress) for the progress bar
- [highlight](https://highlightjs.org/) for the code highlighting 
- [fitvid](http://fitvidsjs.com/) for improving embedded videos
