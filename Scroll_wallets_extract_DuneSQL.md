## To retrieve all wallets from Scroll blockchain using Dune Analytics:

```sql
SELECT 
    "from" as wallet
FROM scroll.transactions
GROUP BY 
    "from"
ORDER BY 
    sum(gas_used) DESC -- To ensure wallets with more points go first
