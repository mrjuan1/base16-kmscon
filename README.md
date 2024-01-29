# kmscon base16 template

A [Base16](http://chriskempson.com/projects/base16/) template for generating a custom colour palette for [kmscon](https://github.com/dvdhrm/kmscon).

# Usage

A [base16 builder](https://github.com/chriskempson/base16#builder-repositories) can be used to generate the colour palette. The output palette can then be added to the end of your kmsconf config file(s).

For example, if using the [base16-builder-bash](https://github.com/mtthlm/base16-builder-bash) base16 builder, you could append the palette to the default kmscon config file (`/etc/kmscon/kmscon.conf`):

```sh
cat theme.yaml | ./base16-builder-bash default.mustache | sudo tee -a /etc/kmscon/kmscon.conf
```

Additionally, each line of the output can be prefixed with a `--` and the `=` replaced with a space and appended to the end of the kmscon command as parameters (eg. `--palette custom --palette-...`).
