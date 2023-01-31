# Managing-private-data
 
const topSecret = Symbol('topSecret'); // our private key; will only be accessible on the scope of
the module file
export class SecretAgent{
 constructor(secret){
 this[topSecret] = secret; // we have access to the symbol key (closure)
 this.coverStory = 'just a simple gardner';
 this.doMission = () => {
 figureWhatToDo(topSecret[topSecret]); // we have access to topSecret
 };
 }
}
