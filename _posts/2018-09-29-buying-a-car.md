---
layout: post
title: A Data Science Approach to Buying a Car
---

Choosing a car is not a quick or easy decision. For me, some of the most important factors to consider are the vehicle's environmental impact, price, its size, and how much I like the look of the car. Another goal is that I like to drive vehicles on the smaller side (no trucks or SUVs for this girl). These considerations narrow my pool to a manageable depth:

> 1. [Toyota Prius](https://www.toyota.ca/toyota/en/vehicles/prius/overview)
> 2. [Toyota Prius c](https://www.toyota.ca/toyota/en/vehicles/prius-c/overview)
> 3. [Toyota Prius Prime](https://www.toyota.ca/toyota/en/vehicles/prius-prime/overview)
> 4. [Nissan Leaf](https://www.nissan.ca/en/electric-cars/leaf)
> 5. [Chevrolet Volt](https://www.chevrolet.ca/volt-electric-car.html)
> 6. [Chevrolet Bolt](https://www.chevrolet.ca/bolt-ev-electric-vehicle.html)
> 7. [Tesla Model 3](https://www.tesla.com/en_CA/model3)
> 8. [Tesla Model S](https://www.tesla.com/en_CA/models)
> 9. [Mini Cooper Electric](https://mini.ca/en/discover/mini-electric)
> 10. [Mini Cooper](https://www.mini.ca/en/mini-f55)
> 11. [Fiat 500e](https://www.fiatusa.com/500e.html)
> 12. [Fiat 500](https://www.fiatcanada.com/en/500)
> 13. [Hyundai IONIQ Hybrid](https://www.hyundaicanada.com/en/showroom/2018/ioniq-hybrid)
> 14. [Hyundai IONIQ Electric](https://www.hyundaicanada.com/en/showroom/2018/ioniq-electric)
> 15. [Hyundai IONIQ Electric Plus](https://www.hyundaicanada.com/en/showroom/2018/ioniq-electric-plus)
> 16. [smart fortwo](https://www.smart.com/ca/en/index/smart-fortwo-electric-drive-453.html)
> 17. [BMW i3](https://www.bmw.ca/en/all-models/bmw-i/i3/2017/at-a-glance.html)
> 18. [Ford Focus EV](https://www.ford.ca/cars/focus/models/focus-electric/?gnav=header-hybrids)
> 19. [Volkswagen e-Golf](https://vwmodels.ca/2018/egolf/)
> 20. [Honda Accord Hybrid](https://www.honda.ca/accord_hybrid)
> 21. [Honda Insight](https://www.honda.ca/insight/2019)
> 22. [Honda Clarity](https://www.honda.ca/clarity)
> 23. [Audi A3 Sportback e-tron](https://www.audi.ca/ca/web/en/models/a3/a3sbetron.html)

This list is mainly comprised of electric and hybrid vehicles, but I have also included the non-electric version of the Fiat 500 as well as the Mini Cooper in my list of considerations, since I really like the way they look. The Mini Electric isn't available yet, but is very likely a car I will want to consider when I'm ready to make this purchase (perhaps in about two years).

There's still a fair amount of variety here, so I'm going to need to quantify what the most important options to assess are.

**The Price**

Price is certainly one of the most driving factors in my decision (pun intended). No matter how amazing a car might be in every way I'd like it to be, if it's insanely expensive, I won't buy it. On the other hand, I hope to have a fancy new job as a Data Scientist by the time I buy this car, so while I will have a budget to adhere to, I also will allow myself the luxury of buying a new car. Thus I am only considering prices of new vehicles, not used.

![center](/figs/2018-09-29-buying-a-car/prices-1.png)

As I mentioned, the Mini Electric isn't actually available yet, so perhaps I shouldn't keep it in the mix at this time. And the Tesla Model S is far more expensive than anything else in my list, so it's got to go as well.

As I mentioned, the Mini Electric isn't actually available yet, so perhaps I shouldn't keep it in the mix at this time. And the Tesla Model S is far more expensive than anything else in my list, so it's got to hit the road as well (puns are funny, yeah?).

**The Price, with Incentives**

The British Columbia Clean Energy Vehicle Program offers pricing incentives for some, but not all, vehicles. Taking these incentives into consideration gives me more relevant information on how much each car will actually cost. Also, it will be nicer to view the cars with the prices ordered.

![center](/figs/2018-09-29-buying-a-car/price incentives-1.png)

Prices range from $22,350 for the Toyota Prius c to $43,750 for the BMW i3. I'm a little surprised that both the BMW and the Fiat 500e are more than the Tesla 3.

**MPG or MPG-e**

Fuel efficiency matters to the planet *and* to my wallet. Gas prices in BC have soared in the last year, so getting good mileage is definitely a significant objective. But how does a person compare an electric vehicle to a hybrid or a regular fuel engine? Isn't this sort of like comparing apples and horses? As it turns out there is a miles per gallon equivalent used by the EPA, which is "a measure of the average distance traveled per unit of energy consumed" according to [Wikipedia.](https://en.wikipedia.org/wiki/Miles_per_gallon_gasoline_equivalent)

![center](/figs/2018-09-29-buying-a-car/mpg-1.png))

Clearly everything above 100mpg blows all the others away, except maybe the Audi. It's unsurprising that the regular fuel cars (the non-electric Fiat and the Mini) are at the bottom of this range, but remarkable by how much, and also that two of the three Priuses on my list are also so low here.

**Range**

I've never owned an electric car before, and I know I'm not alone in being concerned with how far can the car go on a charge (if it's a fully electric), or on a charge and one tank of gas (if it's a plug-in hybrid). This element is moot for the two fuel cars on my list, but worth exploring for all the rest.

![center](/figs/2018-09-29-buying-a-car/range-1.png))

It's notable that the smart fortwo, while it got a high mpg-e rating, can't go very far between charges. Most of my commuting is done within Vancouver, but I certainly want the option to take a road trip. There's quite a range here, and I won't seriously consider buying any vehicle that can't go at least 100 miles.

**Size**

Size is also key, and so any vehicle in a compact class or smaller is going to be more desirable than a mid-size or larger. That said, I don't really want a 2-seater, as I worry it would be limiting in certain circumstances.

**The Analysis**

So, how do I put all these different factors together to see which car is the best? For each category I'll assign a rank and corresponding points, with 1 being the best, and therefore the lowest point score showing the most desirable car.

For all of the above graphs, the ranks are clearly defined. For size and the overall aesthetic of the car, I'll have to insert my own opinionated points system to these.

These different variables are all equally important to me, with the exception of mileage, so I'll weight that a bit more heavily. Thus a final score for each car will be:

$$
Score = Points_{price} + 2 \times Points_{mpg} + Points_{range} + Points_{size} + Points_{aesthetics}
$$

**The Results**

![center](/figs/2018-09-29-buying-a-car/scores-1.png))

The Toyota Prius Prime is the clear winner here. It's a little more than $30k, gets outstanding mileage and range, is compact and cute to boot. It's final score came in at 5.3 points, well ahead of the runner-up Hyundai IONIQ Electric Plus with 9.3 points. Prices may change in the future, but if I were to buy this car today, the Prius Prime is the best choice.


## Additional References

- [BC Clean Energy Vehicle Program Incentives](https://www.plugndrive.ca/discover-electric-vehicles/electric-cars-available-in-canada/)
- [Vehicle Size Class](https://en.wikipedia.org/wiki/Vehicle_size_class)
- [Fuel Economy Ratings](https://www.fueleconomy.gov/feg/findacar.shtml)
