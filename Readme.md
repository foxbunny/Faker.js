# faker.js - generate massive amounts of fake data in the browser and node.js

<img src = "http://imgur.com/KiinQ.png" border = "0">

## USAGE

### browser

```html
<script src = "faker.js" type = "text/javascript"></script>
<script>
  var randomName = faker.Name.findName(); // Caitlyn Kerluke
  var randomEmail = faker.Internet.email(); // Rusty@arne.info
  var randomCard = faker.Helpers.createCard(); // random contact card containing many properties
</script>
```
      
### node.js

```javascript
var faker = require('./faker');
var randomName = faker.Name.findName(); // Rowan Nikolaus
var randomEmail = faker.Internet.email(); // Kassandra.Haley@erich.biz
var randomCard = faker.Helpers.createCard(); // random contact card containing many properties
```
      
## API

* `faker.Name`
  * `.firstName()`
  * `.firstNameFemale()`
  * `.firstNameMale()`
  * `.lastName()`
  * `.findName()`
* `faker.Address`
  * `.zipCode()`
  * `.zipCodeFormat()`
  * `.city()`
  * `.streetName()`
  * `.streetAddress()`
  * `.secondaryAddress()`
  * `.brState()`
  * `.ukCounty()`
  * `.ukCountry()`
  * `.usState()`
  * `.latitude()`
  * `.longitude()`
  * `.PhoneNumber()`
  * `.phoneNumber()`
  * `.phoneNumberFormat()`
* `faker.Internet`
  * `.email()`
  * `.userName()`
  * `.domainName()`
  * `.domainWord()`
  * `.ip()`
  * `.color()`
* `faker.Company`
  * `.suffixes()`
  * `.companyName()`
  * `.companySuffix()`
  * `.catchPhrase()`
  * `.bs()`
* `faker.Image`
  * `.avatar()`
  * `.imageUrl()`
  * `.abstractImage()`
  * `.animals()`
  * `.business()`
  * `.cats()`
  * `.city()`
  * `.food()`
  * `.nightlife()`
  * `.fashion()`
  * `.people()`
  * `.nature()`
  * `.sports()`
  * `.technics()`
  * `.transport()`
* `faker.Lorem`
  * `.words()`
  * `.sentence()`
  * `.sentences()`
  * `.paragraph()`
  * `.paragraphs()`
* `faker.Helpers`
  * `.randomNumber()`
  * `.randomize()`
  * `.slugify()`
  * `.replaceSymbolWithNumber()`
  * `.shuffle()`
  * `.createCard()`
  * `.userCard()`
* `faker.Tree`
  * `.clone()`
  * `.createTree()`
* `faker.Date`
  * `.past()`
  * `.future()`
  * `.between()`
  * `.recent()`
* `faker.random`
  * `.number()`
  * `.array_element()`
  * `.city_prefix()`
  * `.city_suffix()`
  * `.street_suffix()`
  * `.br_state()`
  * `.br_state_abbr()`
  * `.us_state()`
  * `.us_state_abbr()`
  * `.uk_county()`
  * `.uk_country()`
  * `.first_name()`
  * `.last_name()`
  * `.name_prefix()`
  * `.name_suffix()`
  * `.catch_phrase_adjective()`
  * `.catch_phrase_descriptor()`
  * `.catch_phrase_noun()`
  * `.bs_adjective()`
  * `.bs_buzz()`
  * `.bs_noun()`
  * `.phone_formats()`
  * `.domain_suffix()`
  * `.avatar_uri()`
* `faker.definitions`
  * `.first_name()`
  * `.last_name()`
  * `.name_prefix()`
  * `.name_suffix()`
  * `.br_state()`
  * `.br_state_abbr()`
  * `.us_state()`
  * `.us_state_abbr()`
  * `.city_prefix()`
  * `.city_suffix()`
  * `.street_suffix()`
  * `.uk_county()`
  * `.uk_country()`
  * `.catch_phrase_adjective()`
  * `.catch_phrase_descriptor()`
  * `.catch_phrase_noun()`
  * `.bs_adjective()`
  * `.bs_buzz()`
  * `.bs_noun()`
  * `.domain_suffix()`
  * `.lorem()`
  * `.phone_formats()`
  * `.avatar_uri()`

## Tests

```shell
npm install .
make test
```

You can view a code coverage report generated in coverage/lcov-report/index.html.

## Authors

### Matthew Bergman & Marak Squires

Heavily inspired by Benjamin Curtis's Ruby Gem [faker](http://faker.rubyforge.org/) and Perl's [Data::faker](http://search.cpan.org/~jasonk/Data-faker-0.07/lib/Data/faker.pm)

```
Copyright (c) 2014 Matthew Bergman & Marak Squires http://github.com/marak/faker.js/

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```
