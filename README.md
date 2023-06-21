# setup-llvm-msvc
GitHub action to set up llvm-msvc


## Use it in your workflow like this:
```
- name: Setup llvm-msvc
  uses: NewWorldComingSoon/setup-llvm-msvc@v1
```        

## Example
```
- name: Setup llvm-msvc
  uses: NewWorldComingSoon/setup-llvm-msvc@v1

- name: Checkout
  uses: actions/checkout@v2
      
- name: Build
  run: |
    cmake -B build -TLLVM-MSVC_v143
    cmake --build build --config Release
```
