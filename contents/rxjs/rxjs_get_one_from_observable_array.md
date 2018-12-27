
---

- https://stackoverflow.com/questions/50454205/get-one-value-from-observable-array

    ```typescript
    getTransaction(id: number): Observable<Transaction>{
        return this.getTransactions().pipe(
            map(txs => txs.find(txn => txn.id === id))
        );
    }
    ```

---

end
