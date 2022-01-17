```
const depthFirstValues = (root) => {
  if(root == null) return [];
  
//   let stack = [ root ];
//   let result = [];
//   while(stack.length > 0){
//     let current = stack.pop();
//     result.push(current.val)
    
//     if(current.right) stack.push(current.right);
//     if(current.left) stack.push(current.left);
//   }
//   return result;
   
  let leftVal = depthFirstValues(root.left) 
  let leftRight = depthFirstValues(root.right) 
  
  return [root.val,...leftVal, ...leftRight]
};







```
