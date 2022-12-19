# Pandora Box DX Games List

Looking through all 3k games on the app itself is cumbersome without a keyboard, so I created this list.

## The data

I took this data: [Pandora Box Game List (Google Sheet)](https://docs.google.com/spreadsheets/d/1lg-tNRRJOOv-6B8iCAlwhHSu2Tqs8QSV7wB4_gSytds/edit#gid=1263250580)

And converted it to JSON: [CSV2JSON](https://csvjson.com/csv2json)

* [Pandora Box DX - 3000 Games List ](https://pandorastoybox.ca/pandora-box-dx-3000-games-list/)

## For removing empty attribute data
```html
<textarea id=o></textarea>
<script>
o.innerHTML = JSON.stringify(arr.map(a => Object.keys(a).reduce((r, attr) => {
  if (a[attr]) r[attr] = a[attr];
  return r;
}, {})));
</script>
```
