关联策略 	等价属性 	说明
OBJC_ASSOCIATION_ASSIGN 	        @property (assign) or @property (unsafe_unretained) 	弱引用关联对象
OBJC_ASSOCIATION_RETAIN_NONATOMIC 	@property (strong, nonatomic) 	                        强引用关联对象，且为非原子操作
OBJC_ASSOCIATION_COPY_NONATOMIC 	@property (copy, nonatomic) 	                        复制关联对象，且为非原子操作
OBJC_ASSOCIATION_RETAIN 	        @property (strong, atomic)                           	强引用关联对象，且为原子操作
OBJC_ASSOCIATION_COPY 	            @property (copy, atomic) 								复制关联对象，且为原子操作

objc_setAssociatedObject 用于给对象添加关联对象，传入 nil 则可以移除已有的关联对象；
objc_getAssociatedObject 用于获取关联对象；
objc_removeAssociatedObjects 用于移除一个对象的所有关联对象。
