# テクノロジー（藤原） 11/1授業

```
seno2:~/workspace $ git clone git@github.com:seno2/lecture-1101.git
Cloning into 'lecture-1101'...
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
seno2:~/workspace $ pry
[1] pry(main)> num = 2
=> 2
[2] pry(main)> if num % 2 == 0
[2] pry(main)*   puts "偶数です。"
[2] pry(main)* end  
偶数です。
=> nil
[3] pry(main)> puts "偶数です。" if num % 2 == 0
偶数です。
=> nil
[4] pry(main)> 
[5] pry(main)> num = 1000
=> 1000
[6] pry(main)> if num >= 1500
[6] pry(main)*   puts "送料無料です。" 
[6] pry(main)*   
[6] pry(main)> if num >= 1500
[6] pry(main)*   puts "送料無料です。"  
[6] pry(main)* elsif 0 < num && num < 1500  
[6] pry(main)*   puts "送料300円です。"  
[6] pry(main)* else  
[6] pry(main)*   puts "入力が間違ってます。" 
[6] pry(main)* end  
送料300円です。
=> nil
[7] pry(main)> num = rand 3
=> 0
[8] pry(main)> case num
[8] pry(main)* when 0  
[8] pry(main)*   puts "吉です。" 
[8] pry(main)* when 1  
[8] pry(main)*   puts "凶です。" 
[8] pry(main)* else  
[8] pry(main)*   puts "大凶です。"  
[8] pry(main)* end  
吉です。
=> nil
[9] pry(main)> def triangle(b, h)
[9] pry(main)*   result = b * h / 2.0
[9] pry(main)*   result  # 返り値は最後の1行  
[9] pry(main)* end  
=> :triangle
[10] pry(main)> triangle(11, 9)  #=> 49.5
=> 49.5
[11] pry(main)> triangle 11, 9   # 括弧を省略した形
=> 49.5
[12] pry(main)> name = gets
aaaa
=> "aaaa\n"
[13] pry(main)> name.chomp!
=> "aaaa"
[14] pry(main)> name
=> "aaaa"
[15] pry(main)> 10.times do |i|
[15] pry(main)*   print i, ", "
[15] pry(main)* end  
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, => 10
[16] pry(main)> 10.times {|i| print i, ", "}
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, => 10
[17] pry(main)> a = ["りんご", "みかん", "ぶどう"]
=> ["りんご", "みかん", "ぶどう"]
[18] pry(main)> a.each do |item|
[18] pry(main)*   puts "おいしい" + item + "だよ"
[18] pry(main)* end  
おいしいりんごだよ
おいしいみかんだよ
おいしいぶどうだよ
=> ["りんご", "みかん", "ぶどう"]
```