# tungumal
Íslensk heiti á ISO 639-2 tungumálakóðum í YAML-skrá.

Skráin [languages.is.yml](languages.is.yml) inniheldur lista yfir heiti tungumála sem hafa fengið úthlutaðan tveggja stafa kóða skv ISO-639 á Íslensku.

## Notkun í Ruby on Rails

Hægt er að setja skránna beint inn í möppuna `./config/locales/` í Ruby on Rails verkefni. Þá er hægt að birta nafn hvers tungumáls út frá kóða með því að nota fallið `I18n.t`:

```ruby
language = 'en'
I18n.t("languages.#{language}")
=> 'Enska'
```

## Vantar eitthvað?

Skráin var skrifuð eftir bestu getu, en ef þú finnur villur eða vilt koma með tillögur að betri nöfnum, þá má senda pull request á https://github.com/aldavigdis/tungumal/.

## Notkunarleyfi

Skráin er gefin út skv. EUPL-leyfinu (sjá skránna [LICENCE](LICENCE)) en það setur m.a. skilyrði að ef þú nýtir þér skránna, t.d. á vef og leiðréttir hana eða breytir þarftu að gefa breytingarnar út og tryggja að upprunalegs höfundar sé getið í lokaafurð veksins sem hún er notuð í.
