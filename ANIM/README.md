## 文本汉化
[SExtractor](https://github.com/satan53x/SExtractor)

## exe汉化

### 1. 修改编码
- 断点 `CreateFontIndirectA`

  ![img001](assets/img001.jpg)

- `80` → `86`

  ![img002](assets/img002.jpg)

### 2. 修改校验边界

- `cmp eax,0x9F` → `cmp eax,0xFE`

  ![img003](assets/img003.jpg)
  
- `cmp ecx,0x9F` → `cmp ecx,0xFE`

  ![img004](assets/img004.jpg)

### 3. 修复全角空格乱码

- `8140` → `A1A1`
  
  ![img005](assets/img005.jpg)
