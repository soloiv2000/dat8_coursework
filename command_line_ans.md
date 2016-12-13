#This is my answer to the command line homework

1.
The data contains records of orders in a food shop. Each row contains 5 columns: the order_id, the quantity of item, the item name, customer's choice about this item and the item price.
code:
head chipotle.tsv
tail chipotle.tsv

2.
1834 orders

3.
4623 lines
code:
wc -l chipotle.tsv

4.
Chicken burrito is more popular
code:
grep -i "chicken burrito" chipotle.tsv|wc -l
output:553
grep -i "steak burrito" chipotle.tsv|wc -l
output:368

5.
Chicken burritos more often have black beans.
code:
grep -i "chicken burrito" chipotle.tsv|grep -i "black beans"|wc -l
output:282
grep -i "chicken burrito" chipotle.tsv|grep -i "pinto beans"|wc -l
output:105

6.
csv_tsv_list
code:
find . -name *.?sv > ../project/csv_tsv_list

7.
The word "dictionary" occurred about 87 times in the whole DAT8 repository.
code:
grep -ri "dictionary" .| wc -l
output:87






