# Templates

Below is a production-ready invoice template example.

---

## Invoice Template

### HTML

<style>
body{
font-family: Inter, Arial;
margin:40px;
}

.header{
display:flex;
justify-content:space-between;
margin-bottom:30px;
border-bottom:2px solid #eee;
padding-bottom:20px;
}

.title{
font-size:32px;
font-weight:bold;
}

table{
width:100%;
border-collapse:collapse;
margin-top:20px;
}

th{
text-align:left;
border-bottom:1px solid #ddd;
padding:10px 0;
}

td{
padding:10px 0;
border-bottom:1px solid #eee;
}

.total{
text-align:right;
font-size:20px;
margin-top:20px;
font-weight:bold;
}
</style>

<div class="header">

<div>
<div class="title">Invoice</div>
<div>{{invoiceNo}}</div>
</div>

<div>
{{company.name}}<br/>
{{company.city}}
</div>

</div>

<table>

<tr>
<th>Item</th>
<th>Qty</th>
<th>Price</th>
<th>Total</th>
</tr>

{{#each items}}

<tr>

<td>{{name}}</td>
<td>{{qty}}</td>
<td>{{price}}</td>
<td>{{total}}</td>

</tr>

{{/each}}

</table>

<div class="total">

Total {{grandTotal}}

</div>

---

## Example JSON

{
"invoiceNo":"INV-1001",

"company":{
"name":"WebSvc",
"city":"Chennai"
},

"items":[
{
"name":"Subscription",
"qty":1,
"price":100,
"total":100
}
],

"grandTotal":100
}
