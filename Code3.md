<a href="https://mayadickson.github.io/Portfolio/">Home</a>


# Keyword combinations for a Google ad
## Creating keywords that target price-sensitive customers
*Pairs a word list, that targets price-sensitive customers, with products that a client wants to sell.*

This is done by:
1. Creating a list of words that a user might use to search for price-sensitive products
2. Making a keywords list
    1. Create an empty list
    2. Create loops that go through the products and words
    3. Append these combinations to the empty list


```python
products = ['sofas', 'convertible sofas', 'love seats', 'recliners', 'sofa beds']
words = ['discount', 'buy', 'shop', 'price', 'promo', 'bargain']

keywords_list = []
for product in products:
    for word in words:
        keywords_list.append([product, product + ' ' + word])
        keywords_list.append([product, word + ' ' + product])

#print to view results
print(keywords_list)
```

    [['sofas', 'sofas discount'], ['sofas', 'discount sofas'], ['sofas', 'sofas buy'], ['sofas', 'buy sofas'], ['sofas', 'sofas shop'], ['sofas', 'shop sofas'], ['sofas', 'sofas price'], ['sofas', 'price sofas'], ['sofas', 'sofas promo'], ['sofas', 'promo sofas'], ['sofas', 'sofas bargain'], ['sofas', 'bargain sofas'], ['convertible sofas', 'convertible sofas discount'], ['convertible sofas', 'discount convertible sofas'], ['convertible sofas', 'convertible sofas buy'], ['convertible sofas', 'buy convertible sofas'], ['convertible sofas', 'convertible sofas shop'], ['convertible sofas', 'shop convertible sofas'], ['convertible sofas', 'convertible sofas price'], ['convertible sofas', 'price convertible sofas'], ['convertible sofas', 'convertible sofas promo'], ['convertible sofas', 'promo convertible sofas'], ['convertible sofas', 'convertible sofas bargain'], ['convertible sofas', 'bargain convertible sofas'], ['love seats', 'love seats discount'], ['love seats', 'discount love seats'], ['love seats', 'love seats buy'], ['love seats', 'buy love seats'], ['love seats', 'love seats shop'], ['love seats', 'shop love seats'], ['love seats', 'love seats price'], ['love seats', 'price love seats'], ['love seats', 'love seats promo'], ['love seats', 'promo love seats'], ['love seats', 'love seats bargain'], ['love seats', 'bargain love seats'], ['recliners', 'recliners discount'], ['recliners', 'discount recliners'], ['recliners', 'recliners buy'], ['recliners', 'buy recliners'], ['recliners', 'recliners shop'], ['recliners', 'shop recliners'], ['recliners', 'recliners price'], ['recliners', 'price recliners'], ['recliners', 'recliners promo'], ['recliners', 'promo recliners'], ['recliners', 'recliners bargain'], ['recliners', 'bargain recliners'], ['sofa beds', 'sofa beds discount'], ['sofa beds', 'discount sofa beds'], ['sofa beds', 'sofa beds buy'], ['sofa beds', 'buy sofa beds'], ['sofa beds', 'sofa beds shop'], ['sofa beds', 'shop sofa beds'], ['sofa beds', 'sofa beds price'], ['sofa beds', 'price sofa beds'], ['sofa beds', 'sofa beds promo'], ['sofa beds', 'promo sofa beds'], ['sofa beds', 'sofa beds bargain'], ['sofa beds', 'bargain sofa beds']]


<a href="https://mayadickson.github.io/Portfolio/Code3.html"<Back to Top>/a<
