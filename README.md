# csc2558-exp
A simple Github Page for A/B testing and randomized experiments

Usage
----
1. Fork this repo so that it appears under your github account.
2. Set up a Github-page environment for the repo. This can be done by accessing "Settings - Pages" and selecting the `main` branch under the "Source" section.
3. Edit the `urls` variable in `index.html` so that it contains the links of your web surveys:
```html
<script type="text/javascript">
    var urls = [
        'https://1nog73d57hz.typeform.com/to/mIA2xmRd',
        'https://1nog73d57hz.typeform.com/to/C7KKx40m',
    ];

    function redirect() {
        var url = urls[Math.floor(Math.random() * urls.length)];
        window.location = url; // redirect
    }
</script>
```
4. Access `https://<user-name>.github.io/csc2558-exp/` to view the published web page.

Experimental Results
----
The experimental results and analysis of this project can be found in the jupyer notebook [here](https://github.com/parulsaini42/Optimzing-Web-Forms-using-A-B-Testing-and-Reinforcement-Learning/blob/main/A-B%20Testing%20%26%20Reinforcement%20Learning.ipynb).
