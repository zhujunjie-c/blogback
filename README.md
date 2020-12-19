# blogback
blog后端
# 12.16新增
## 新增category：
* 新增文章时需要新增category字段（完成）
* 新增category时需要判断category是否已存在，需要对category进行一个查询。（直接使用插入，若是失败则说明可能已存在）
* 在对文章进行初步获取时需要对文章按category分类（可以由前端完成）
* 文章的字段也需要添加一个category字段，字段还是用categoryID（完成）	
* category的增删查改（完成）
* 文章修改时也需要对category进行修改（完成）
## 需要测试：
* 修改category后，立刻进行文章的category修改，看是否会成功
* 前端添加相应功能

#12.19修改
* 增加中间件：数据增删改 通过中间件验证 在header增加以下字段
  * puberaccount
  * token
    
    共同用于验证token，不使用body，因为body内的内容只能读一次
    在中间件中使用普通的postform无法读取
 * 增加需求文档
 * 增加数据库结构文档
 * 测试增加博文 成功
 * 测试更新博文 成功
 * 测试分类相关api 
    * 修改 成功
    * 新增 成功
    * 查询 成功
 
