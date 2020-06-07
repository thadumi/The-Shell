# The Shell

Minimalistic dark color theme for [Ghost](http://github.com/tryghost/ghost/) platform. Based on [The Shell](https://github.com/mityalebedev/The-Shell)

![image](https://user-images.githubusercontent.com/1761114/55421430-dc7f8e80-5581-11e9-9db8-ad3071f09098.png)

Live here: [https://thadumi.com](https://thadumi.com/).

----

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
- fitvid
- highlight 
