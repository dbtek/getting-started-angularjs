##Example: Data Binding

<pre><code data-trim contenteditable>
<div ng-app ng-init="qty=1;cost=2">
  <b>Invoice:</b>
  <div>
    Quantity: <input type="number" ng-model="qty" required >
  </div>
  <div>
    Costs: <input type="number" ng-model="cost" required >
  </div>
  <div>
    <b>Total:</b> {{qty * cost | currency}}
  </div>
</div>
</code></pre>

<iframe src="examples/data-bind/index.html"></iframe>