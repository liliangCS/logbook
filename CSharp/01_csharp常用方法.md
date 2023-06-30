## byte数组和string互相转化
- `string str = System.Text.Encoding.UTF8.GetString(bytes);` 
- `byte[] decBytes = System.Text.Encoding.UTF8.GetBytes(str);`

## json字符串和对象互相转化
- `Newtonsoft.Json.JsonConvert.SerializeObject`
- `Newtonsoft.Json.JsonConvert.DeserializeObject`
