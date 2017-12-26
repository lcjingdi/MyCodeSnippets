## MyOCCodeSnippets USAGE



### 代理方法

控件名+delegate+分组

> tableview_delegate_display: 

```objective-c
// Display customization
- (void)tableView:(UITableView *)tableView willDisplayCell:(UITableViewCell *)cell forRowAtIndexPath:(NSIndexPath *)indexPath {
    <#code#>
}
- (void)tableView:(UITableView *)tableView willDisplayHeaderView:(UIView *)view forSection:(NSInteger)section NS_AVAILABLE_IOS(6_0) {
    <#code#>
}
- (void)tableView:(UITableView *)tableView willDisplayFooterView:(UIView *)view forSection:(NSInteger)section NS_AVAILABLE_IOS(6_0) {
    <#code#>
}
- (void)tableView:(UITableView *)tableView didEndDisplayingCell:(UITableViewCell *)cell forRowAtIndexPath:(NSIndexPath*)indexPath NS_AVAILABLE_IOS(6_0) {
    <#code#>
}
- (void)tableView:(UITableView *)tableView didEndDisplayingHeaderView:(UIView *)view forSection:(NSInteger)section NS_AVAILABLE_IOS(6_0) {
    <#code#>
}
- (void)tableView:(UITableView *)tableView didEndDisplayingFooterView:(UIView *)view forSection:(NSInteger)section NS_AVAILABLE_IOS(6_0) {
    <#code#>
}
```



### 数据源

控件名+datasource+required / 控件名+datasource+optional

> tableview_datasource_required

```objective-c
// required
- (NSInteger)tableView:(UITableView *)tableView numberOfRowsInSection:(NSInteger)section {
    <#code#>
}
- (UITableViewCell *)tableView:(UITableView *)tableView cellForRowAtIndexPath:(NSIndexPath *)indexPath {
    <#code#>
}
// optional
- (NSInteger)numberOfSectionsInTableView:(UITableView *)tableView {
    <#code#>
}
- (nullable NSString *)tableView:(UITableView *)tableView titleForHeaderInSection:(NSInteger)section {
    <#code#>
}
- (nullable NSString *)tableView:(UITableView *)tableView titleForFooterInSection:(NSInteger)section {
    <#code#>
}
// Editing
- (BOOL)tableView:(UITableView *)tableView canEditRowAtIndexPath:(NSIndexPath *)indexPath {
    <#code#>
}
- (BOOL)tableView:(UITableView *)tableView canMoveRowAtIndexPath:(NSIndexPath *)indexPath {
    <#code#>
}
// Index
- (nullable NSArray<NSString *> *)sectionIndexTitlesForTableView:(UITableView *)tableView {
    <#code#>
}
- (NSInteger)tableView:(UITableView *)tableView sectionForSectionIndexTitle:(NSString *)title atIndex:(NSInteger)index {
    <#code#>
}
- (void)tableView:(UITableView *)tableView commitEditingStyle:(UITableViewCellEditingStyle)editingStyle forRowAtIndexPath:(NSIndexPath *)indexPath {
    <#code#>
}
- (void)tableView:(UITableView *)tableView moveRowAtIndexPath:(NSIndexPath *)sourceIndexPath toIndexPath:(NSIndexPath *)destinationIndexPath {
    <#code#>
}
```



### 快速创建

##### 方法快速创建

分类_function

> lifecycle_function

```objective-c
- (void)viewWillAppear:(BOOL)animated {
    [super viewWillAppear:animated];
}
- (void)viewDidAppear:(BOOL)animated {
    [super viewDidAppear:animated];
}
- (void)viewWillDisappear:(BOOL)animated {
    [super viewWillDisappear:animated];
}
- (void)viewDidDisappear:(BOOL)animated {
    [super viewDidDisappear:animated];
}
- (void)viewDidLoad {
    [super viewDidLoad];
}
- (void)dealloc {
    
}
```





### 属性

x+内存管理策略

> xweak: @property (nonatomic, weak) <#type#> *<#name#>;



### 延时加载

Lazy

> lazy

```objective-c
- (<#property type#> *)<#property name#> {
    if (_<#property name#> == nil) {
        _<#property name#> = [[<#property type#> alloc] init];
    }
    return _<#property name#>;
}
```



### 注释风格

pm

> pm

```objective-c
#pragma mark - Lifecycle
#pragma mark - NSObject
#pragma mark - NSCopying
#pragma mark - Function
#pragma mark - IBActions
#pragma mark - Events
#pragma mark - Override
#pragma mark - Public
#pragma mark - Private
#pragma mark - Protocol conformance
#pragma mark - Tool
#pragma mark - Lazy
```

