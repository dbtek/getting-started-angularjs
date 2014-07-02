##Example: Controller
index.html

```
<div ng-app="invoice" ng-controller="InvoiceController">
  <b>Invoice:</b>
  <div>
    Quantity: <input type="number" ng-model="qty" required >
  </div>
  <div>
    Costs: <input type="number" ng-model="cost" required >
    <select ng-model="inCurr">
      <option ng-repeat="c in currencies">{{c}}</option>
    </select>
  </div>
  <div>
    <b>Total:</b>
    <span ng-repeat="c in currencies">
      {{total(c) | currency:c}}
    </span>
    <button class="btn" ng-click="pay()">Pay</button>
  </div>
</div>
```