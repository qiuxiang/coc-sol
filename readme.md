[npm]: https://www.npmjs.com/package/coc-solidity
[npm-badge]: https://img.shields.io/npm/v/coc-solidity.svg

# coc-solidity [![npm-badge]][npm]

coc.nvim extension for solidity. Language server provided by [solidity-ls](https://github.com/qiuxiang/solidity-ls).

<img width="276" alt="image" src="https://user-images.githubusercontent.com/1709072/159026514-4d178c66-336c-46c3-b647-37d8ed048568.png"><img width="276" alt="image" src="https://user-images.githubusercontent.com/1709072/159026797-af4de669-49ff-4036-b6b0-0ea42a68a019.png"><img width="276" alt="image" src="https://user-images.githubusercontent.com/1709072/159030410-65a68fe6-bc77-45e2-aa8a-b305fbb01b17.png">

**[solidity-ls](https://github.com/qiuxiang/solidity-ls) currently has no tolerance.**
Means that some completions will only work if sources are no syntax error.

For example:

```solidity
// should not work
msg.
   ^

// should work fine
msg.;
   ^
```


# Features

- completion
  - <details>
      <summary>local variables, state variables, functions</summary>
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159023964-24d7459f-3dfd-4b5e-8b05-252cb1ea106c.png">
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159026179-88253d5f-3391-4165-99f3-0a8a303c7775.png">
    </details>
  - <details>
      <summary>contracts</summary>
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159024159-e8993183-c7e1-476a-ae87-91a0bf9b3c89.png">
    </details>
  - <details>
      <summary>globally variables and it's members</summary>
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159024903-c30c5dbc-b6d8-4c7f-8d04-18e61140a487.png">
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159025055-0ef5e754-761d-4d6b-8236-bce2bd55f9be.png">
    </details>
  - <details>
      <summary>struct members</summary>
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159025910-1044db6b-281a-4e86-8099-7dba3bc25e5f.png">
    </details>
  - <details>
      <summary>external contract functions</summary>
      <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159026514-4d178c66-336c-46c3-b647-37d8ed048568.png">
    </details>
- <details>
    <summary>diagnostics</summary>
    <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159026797-af4de669-49ff-4036-b6b0-0ea42a68a019.png">
    <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159026860-13649b4d-8e5a-447c-8c4d-09b18e8ec7d4.png">
  </details>
- <details>
    <summary>hover documention</summary>
    <img width="645" alt="image" src="https://user-images.githubusercontent.com/1709072/159030410-65a68fe6-bc77-45e2-aa8a-b305fbb01b17.png">
  </details>
- formatting (by prettier-plugin-solidity)
- go to definition

## Install

`:CocInstall coc-solidity`

# TODO

- [ ] code actions
- [ ] rename
