![get-my-invoices](https://www.getmyinvoices.com/wp-content/uploads/2016/04/logo_login.png)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FNerzal%2Fgogmi.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FNerzal%2Fgogmi?ref=badge_shield)

# gogmi is a golang-library for getmyinvoices.com

Here you can find the API-documentation: https://api.getmyinvoices.com/accounts/v2/doc/#

## Already implemented

✔ list supplieres  
✔ get specific supplier  
✔ list invoices  
✘ upload new invoice  
✘ update invoice  
✔ get country list  
✘ add custom supplier  
✘ update custom supplier  
✘ delete custom supplier  

## Getting started

```golang
client := gogmi.GMI{
    APIVersion: "v1",
    APIKey:     "your-API-Key",
}
suppliers, err := client.ListSuppliers()
if err != nil {
    t.Error(err)
}

// do something with suppliers
```



## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FNerzal%2Fgogmi.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2FNerzal%2Fgogmi?ref=badge_large)