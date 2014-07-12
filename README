###一个kissy的LazyLoad组件

###版本：v0.1

###调用：

	KISSY.config({
		packages: {
			'my': {
				combine: false,
				debug: true,
				ignorePackageNameInUri:true,
				base: './pkg/v0.0.1/'
			}
		}
	});

	KISSY.use('my/lazyload', function(S, Lazyload) {
		var lazyLoad = new Lazyload(['#floor1', '#floor3'], {
			lazyAttr: 'data-ks-lazyload',
			lazyCls: 'cls-ks-lazyload',
			delay: 500,
			threshold: 10,
			scrollX: false,
			scrollY: true,
			callback: [
				{ele: '#floor1', fn: function(){ console.log('callback 1'); } },
				{ele: '#floor2', fn: function(){ console.log('callback 2'); } }
			]
		});
	});


###配置：

    /**
     *  懒加载图片存放src的自定义属性
     */		
	lazyAttr: 'data-ks-lazyload'

    /**
     *  用以标识懒区域的class
     */			
	lazyCls: 'cls-ks-lazyload'

    /**
     *  距离视口触发懒加载的阈值
     */			
	threshold: 100

    /**
     *  触发懒加载后的加载延迟     
     */	
	delay: 400

    /**
     *  在水平方向进行懒加载
     */			
	scrollX: false

    /**
     *  在垂直方向进行懒加载
     */			
	scrollY: true

    /**
     *  进行懒加载的对象数组，如{ele: '#div', fn: callbackFn}
     */			
	callback: []


###api：

- updateLazyElement，更新懒元素 _（注：懒元素并不会自动更新，如果实例化后 dom 的改变导致懒元素发生改变，需要调用该函数进行更新）_



