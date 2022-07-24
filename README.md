# JMeter
apache-jmeter-5.5に対する修正モジュール  
・javaのURLEncoder/Decoderを使用せずapacheのorg.apache.commons.codec.net.URLCodecを使用する修正  
　Content-Typeのmime typeがapplication/x-www-form-urlencodedの場合にcharsetが指定されないと  
　記録されたリクエストの日本語が文字化けする不具合の修正  
　org\apache\jmeter\functions  
　org\apache\jmeter\protocol\http\sampler  
　org\apache\jmeter\protocol\http\util  
・Proxyの「Recording's default encoding」を記録の途中で変更可能にする修正  
　org\apache\jmeter\protocol\http\proxy  
・上記２つの修正したモジュールを入れ替えたjar  
　lib/ext  
