1. values added: 20
2. final result: 20
3. values added: 20
4. ReferenceError because let result had block scope and line 13 is outside the block
5. TypeError because we aren't allowed to reassign const variables, which was done on line 7
6. The previous error would stop the function, but regardless this line would throw a ReferenceError because const result had block scope and line 13 is outside the block
