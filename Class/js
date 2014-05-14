(function(){
    this.Class = function(){};
    this.Class.prototype.store = {};
    this.Class.prototype.set = function(key, value){
        this.store[key] = value;
    };
    this.Class.prototype.get = function(key){
        return this.store.hasOwnProperty(key) ? this.store[key] : null;
    };
    Class.extend = function(args){
        var prototype = new this();
        for(var name in args){
            prototype[name] = args[name];
        }
        Class.prototype = prototype;
        Class.prototype.constructor = Class;
        Class.extend = arguments.callee;
        return Class;
    };
})();
