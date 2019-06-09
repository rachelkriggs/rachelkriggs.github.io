---
layout: post
title: A Data Science Approach to Buying a Car
tags: [data-science, analysis]
---

<img src="/images/car-fog.jpg" class="fit image">

Choosing a car is not a quick or easy decision. For me, some of the most important factors to consider are the vehicle's environmental impact, price, its size, and how much I like its design. Another aspect is that I like to drive vehicles on the smaller side (no trucks or SUVs for this girl). These considerations narrow my pool to a manageable depth of 23 different vehicles:

1. [Toyota Prius](https://www.toyota.ca/toyota/en/vehicles/prius/overview)
2. [Toyota Prius c](https://www.toyota.ca/toyota/en/vehicles/prius-c/overview)
3. [Toyota Prius Prime](https://www.toyota.ca/toyota/en/vehicles/prius-prime/overview)
4. [Nissan Leaf](https://www.nissan.ca/en/electric-cars/leaf)
5. [Chevrolet Volt](https://www.chevrolet.ca/volt-electric-car.html)
6. [Chevrolet Bolt](https://www.chevrolet.ca/bolt-ev-electric-vehicle.html)
7. [Tesla Model 3](https://www.tesla.com/en_CA/model3)
8. [Tesla Model S](https://www.tesla.com/en_CA/models)
9. [Mini Cooper Electric](https://mini.ca/en/discover/mini-electric)
10. [Mini Cooper](https://www.mini.ca/en/mini-f55)
11. [Fiat 500e](https://www.fiatusa.com/500e.html)
12. [Fiat 500](https://www.fiatcanada.com/en/500)
13. [Hyundai IONIQ Hybrid](https://www.hyundaicanada.com/en/showroom/2018/ioniq-hybrid)
14. [Hyundai IONIQ Electric](https://www.hyundaicanada.com/en/showroom/2018/ioniq-electric)
15. [Hyundai IONIQ Electric Plus](https://www.hyundaicanada.com/en/showroom/2018/ioniq-electric-plus)
16. [smart fortwo](https://www.smart.com/ca/en/index/smart-fortwo-electric-drive-453.html)
17. [BMW i3](https://www.bmw.ca/en/all-models/bmw-i/i3/2017/at-a-glance.html)
18. [Ford Focus EV](https://www.ford.ca/cars/focus/models/focus-electric/?gnav=header-hybrids)
19. [Volkswagen e-Golf](https://vwmodels.ca/2018/egolf/)
20. [Honda Accord Hybrid](https://www.honda.ca/accord_hybrid)
21. [Honda Insight](https://www.honda.ca/insight/2019)
22. [Honda Clarity](https://www.honda.ca/clarity)
23. [Audi A3 Sportback e-tron](https://www.audi.ca/ca/web/en/models/a3/a3sbetron.html)

This list is mainly comprised of electric and hybrid vehicles, but I have also included the non-electric version of the Fiat 500 as well as the Mini Cooper in my list of considerations, since I think they're really stylish. The Mini Electric isn't available yet, but is very likely a car I will want to consider when I'm ready to make this purchase (perhaps in about two years).

There's still a fair amount of variety here, so I'm going to need to quantify what the most important options to assess are.

## **The Price**

Price is certainly one of the most driving factors in my decision (pun intended). No matter how amazing a car might be in every way I'd like it to be, if it's insanely expensive, I won't buy it. On the other hand, I hope to have a fancy new job as a Data Scientist by the time I buy this car, so while I will have a budget to adhere to, I also will allow myself the luxury of buying a new car. Thus I am only considering prices of new vehicles, not used.

<img src="/figs/2018-09-29-buying-a-car/prices-1.png" class="fit image">

As I mentioned, the Mini Electric isn't actually available yet, so perhaps I shouldn't keep it in the mix at this time. And the Tesla Model S is far more expensive than anything else in my list, so it's got to hit the road as well (puns are funny, yeah?).

## **The Price, with Incentives**

The [British Columbia Clean Energy Vehicle Program](https://www.plugndrive.ca/discover-electric-vehicles/electric-cars-available-in-canada/) offers pricing incentives for some, but not all, vehicles. Taking these incentives into consideration gives me more relevant information on how much each car will actually cost. Also, it will be nicer to view the cars with the prices ordered.

<img src="/figs/2018-09-29-buying-a-car/price-incentives-1.png" class="fit image">

Prices range from $22,350 for the Toyota Prius c to $43,750 for the BMW i3. I'm a little surprised that the Tesla 3 isn't the most expensive.

## **MPG or MPG-e**

Fuel efficiency matters to the planet *and* to my wallet. Gas prices in BC have soared in the last year, so getting good mileage is definitely a significant objective. But how does a person compare an electric vehicle to a hybrid or a regular fuel engine? Isn't this sort of like comparing apples and horses? As it turns out there is a miles per gallon equivalent used by the EPA, which is "a measure of the average distance traveled per unit of energy consumed" according to [Wikipedia.](https://en.wikipedia.org/wiki/Miles_per_gallon_gasoline_equivalent)

<img src="/figs/2018-09-29-buying-a-car/mpg-1.png" class="fit image">

Clearly everything above 100mpg blows away the rest of the field, except maybe the Audi. It's unsurprising that the regular fuel cars (the non-electric Fiat and the Mini) are at the bottom of this range, but remarkable by how much, and also that two of the three Priuses on my list are also so low here.

## **Range**

I've never owned an electric car before, and I know I'm not alone in being concerned with how far the car can go on a charge (if it's a fully electric), or on a charge and one tank of gas (if it's a plug-in hybrid). This element is moot for the two fuel cars on my list (the Fiat 500 and the Mini Cooper), but worth exploring for all the rest.

<img src="/figs/2018-09-29-buying-a-car/range-1.png" class="fit image">

It's notable that the smart fortwo, while it got a high mpg-e rating, can't go very far between charges. Most of my commuting is done within Vancouver, but I certainly want the option to take a road trip. There's quite a range here, and I won't seriously consider buying any vehicle that can't go at least 100 miles.

As an aside, yes, I'm aware that I'm talking about buying this car in Canada and yet I've used miles for both efficiency and range, rather than kilometers. What can I tell you -- I'm the one making this decision, so you're going to have to trust that this is the best way for me to understand the data! I'm American; my brain doesn't have to think what mpg means, but it does for km.

## **Size**

Size is also key, and so any vehicle in a compact class or smaller is going to be more desirable than a mid-size or larger. That said, I don't really want a 2-seater, as I worry it would be limiting in certain circumstances.

I'll assign a points system. There are seven vehicle classes for my list of cars, some of which I consider equally desirable. Since 4 of the classes are tied for best rank, they will all get a 1, and the remaining classes get the next scores of 5, 6, and 7.

| class | rank of desirability |
| ----- | -------------------: |
| compact, subcompact, supermini, city car | 1 |
| mid-size | 5 |
| two-seater | 6 |
| small station wagon | 7 |

Which gives my list of cars the following points for size:

| make and model              | vehicle class       | points for size |
| :-------------------------- | :------------------ | -------: |
| Audi A3 Sportback e-tron    | compact             |        1 |
| BMW i3                      | subcompact          |        1 |
| Chevrolet Volt              | compact             |        1 |
| Fiat 500e                   | city car            |        1 |
| Fiat 500                    | city car            |        1 |
| Ford Focus EV               | compact             |        1 |
| Honda Accord Hybrid         | compact             |        1 |
| Mini Cooper 5-door          | supermini           |        1 |
| Toyota Prius                | compact             |        1 |
| Toyota Prius c              | subcompact          |        1 |
| Toyota Prius Prime          | compact             |        1 |
| Volkswagen e-Golf           | compact             |        1 |
| Honda Clarity               | mid-size            |        5 |
| Honda Insight               | mid-size            |        5 |
| Hyundai IONIQ Electric      | mid-size            |        5 |
| Hyundai IONIQ Electric Plus | mid-size            |        5 |
| Hyundai IONIQ Hybrid        | mid-size            |        5 |
| Nissan LEAF                 | mid-size            |        5 |
| Tesla Model 3               | mid-size            |        5 |
| smart fortwo                | two-seater          |        6 |
| Chevrolet Bolt              | small station wagon |        7 |

## **Style**

Since design also factors into my decision, I'll also assign a points system for aesthetics. 1 is again the best, and there were a few ties which are reflected in duplicate scores:

| make and model              | aesthetic score |
| :-------------------------- | -------------: |
| Fiat 500e                   |              1 |
| Fiat 500                    |              1 |
| Mini Cooper 5-door          |              1 |
| BMW i3                      |              4 |
| Toyota Prius                |              5 |
| Toyota Prius c              |              5 |
| Toyota Prius Prime          |              5 |
| Nissan LEAF                 |              8 |
| Chevrolet Bolt              |              9 |
| Chevrolet Volt              |             10 |
| Hyundai IONIQ Electric      |             10 |
| Hyundai IONIQ Electric Plus |             10 |
| Hyundai IONIQ Hybrid        |             10 |
| Honda Accord Hybrid         |             14 |
| Honda Insight               |             14 |
| Ford Focus EV               |             16 |
| Honda Clarity               |             16 |
| smart fortwo                |             16 |
| Tesla Model 3               |             16 |
| Audi A3 Sportback e-tron    |             20 |
| Volkswagen e-Golf           |             21 |

## **The Analysis**

Now I need to put all these different factors together to find out which car is the best overall. In all categories the lowest rank/point score is the best; therefore the lowest overall score wins.

These different variables are all equally important to me, with the exception of mileage, so I'll weight that a bit more heavily. Thus a final score for each car will be:

<img src="/figs/2018-09-29-buying-a-car/equation.png" class="fit image">

## **The Results**

<br/><br/>

<img src="/figs/2018-09-29-buying-a-car/scores-1.png" class="fit image">

| make and model              | final score |
| :-------------------------- | -----------: |
| Toyota Prius Prime          |          4.0 |
| Hyundai IONIQ Electric Plus |          6.8 |
| Hyundai IONIQ Electric      |          8.4 |
| Toyota Prius                |          9.8 |
| Hyundai IONIQ Hybrid        |         10.2 |
| Nissan LEAF                 |         10.4 |
| Toyota Prius c              |         10.4 |
| Volkswagen e-Golf           |         10.6 |
| Chevrolet Bolt              |         11.2 |
| Fiat 500e                   |         11.4 |
| Chevrolet Volt              |         11.8 |
| BMW i3                      |         12.0 |
| Tesla Model 3               |         12.6 |
| smart fortwo                |         13.0 |
| Honda Clarity               |         13.2 |
| Honda Insight               |         13.2 |
| Fiat 500                    |         13.3 |
| Mini Cooper 5-door          |         13.5 |
| Honda Accord Hybrid         |         13.6 |
| Ford Focus EV               |         14.8 |
| Audi A3 Sportback e-tron    |         15.0 |

| make and model     | vehicle class | mpg or mpge equivalent | price after incentives | final score |
| :----------------- | :------------ | ---------------------: | ---------------------: | ----------: |
| Toyota Prius Prime | compact       |                    133 |                  30490 |           4 |


The Toyota Prius Prime is the clear winner here. It's a little more than $30k, gets outstanding mileage and range, is compact and cute to boot. It's final score came in at 4 points, ahead of the runner-up Hyundai IONIQ Electric Plus with 6.8 points. Prices may change in the future, but if I were to buy this car today, the Prius Prime is the best choice.


#### Additional References

- [Vehicle Size Class](https://en.wikipedia.org/wiki/Vehicle_size_class)
- [Fuel Economy Ratings](https://www.fueleconomy.gov/feg/findacar.shtml)
- Photo by [Regis F](https://unsplash.com/@herosordinaires?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/)
