Describe: Pizza(toppings, size, price);
Test: It should output value of each property when called upon. 
code: function Pizza() {
    this.size = undefined; 
    this.toppings = undefined; 
    this.sizePrice = 0; 
    this.toppingsPrice = 0;
    this.totalPrice = 0;  
    let output = new Pizza ('medium', 'cheese', 12, 3);
}
Expect((output.size).toEqual('medium'));

Describe: Pizza.prototype.addsize() 
Test: It should take input size and assign cost based on size. 
code: Pizza.prototype.addSize = function(size) {
    this.size = size;
    if(this.size === 'small'){
        this.sizePrice = 10; 
    } else if (this.size === 'medium'){
        this.sizePrice = 15;
    } else  {
        this.sizePrice === 20;
    } 
}
Expect:(addsize('medium').toEqual(size))


