# CIRKIT-1 OperatingManual
20160601徳安一

Index: 

 *1.構成 
 *2.運用法 
 *3.整備法 
 *4.引き継ぎ事項 
  
# 1:構成

Ubuntu14.04LTS搭載ノート + ゲームパッド(PS3)
ラズベリーパイ2B+  
アルディーノUNO  
本体基板  

# 2:運用法

Ubuntu14.04LTSにて propo を実行,ゲームパッド接続 
ラズベリーパイ2B+は server を実行,コントローラーとして作動 

Ubuntu から ラズベリーパイ( server 起動中)の ip アドレスへ接続する.
ip アドレスの通知には, 私の Autologger が便利だと思いますね(宣伝)
通信に成功すれば, ゲームパッドからコントロールできるようになる.

Arduinoはラズベリーパイと接続,デジタル通信(ピン配置はpinNoと同様なのでピン配置表とソースコードより配置せよ)  
さらにモーターコントローラ(2016時点でSERVREXコントローラ*引き継ぎ事項を見よ)をタグ付きの8口ワイヤとピンで直結,通信を確認  

点火前に緊急停止スイッチを押下,爾後点火し,基板タクトスイッチを自動制御モードへ移行.

# 3:整備法  
往々にして基板が壊れる.信号がはいってない時はまずここを疑う.断線は茶飯インシデント.ホットボンドは信用するな,その下で切れてる・・・  

# 4:引き継ぎ事項  
SERVREXが逆接続のミス(ぼくのせいです)で不調となっている.いつか予算をおろしてもらうか,アナログ波形をまともに発信できる回路を組み立てるより他にないので注意.