# myPinchZoom
针对项目需求，对pinchzoom的改进版

## dom结构
```html
      <div v-show="currentPage===2" class="page select-frame1" style="display:none">
        <div ref="resultImg" class="select-frame1-item">
          <div class="wrapper" :class="{'overflow-hidden': !creatingImg}" id="wrapper">
            <img :src="imgData" ref="photo" class="photo parent-photo" id="photo">
          </div>
        </div>
      </div>
```
## js代码
```js
     initDragAndScale() {
              let img = document.querySelector('.photo');
              this.pz = new PinchZoom(img, {
                imageSelector: 'photo'
              });
            },
```
