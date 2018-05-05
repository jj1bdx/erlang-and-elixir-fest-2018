# Erlang & Elixir Fest 2018 talk repository

16-JUN-2018 Akihabara, Tokyo, Japan

## タイトル

共有からメッセージパッシングへ: Erlang/OTPやElixirと歩んだこの10年

## 概要

講演者が最初にErlangに触れたのは2008年。今年で10年が経過した。この間講演者がErlangから学んだものは、関数型プログラミングやライブラリシステムOTPのもたらす安全な
並行プログラミング原則など多岐にわたる。それらの中で最も重要なものは、極力共有や参照を排し、明示的なディープコピーあるいはメッセージパッシングのみを使うという頑固ともいえる設計哲学である。

本講演では、CやC++、C#といった従来の言語とのセマンティクスを比較しながら、Erlang/OTPやElixirが目指すものと目指さないことを概観し、 Lagom är bäst （ほどほどにちょうど良いくらいが一番良い）というスウェーデンの価値観を体現したErlangの良さ、それを継承して発展しているElixir、そしてそれらのコミュニティを含めた今後の展望についての考察を示す。

## Core issues

### Performance or safety?

* Programmers strive for performance / 性能のあくなき追求
* Performance and safety are tradeoffs / 性能と安全はトレードオフの関係にある
* Programmers are always cutting corners / プログラマは常にどうやって手抜きをするかを目指してきた
* Performance are essential for popularity and money / 人気とお金を得るためには性能はなくてはならない
* People pay less money for security and privacy than for performance and features / 人々がお金を払うのは性能と機能に対してでありセキュリティやプライバシーのためではない

### Are all languages equal and equivalent?

* Programmers assume cutting corners are always possible / プログラマは常に手抜きができると仮定している
* Assumption for cutting corners means that there are always *equivalent* shorter and faster algorithms for all algorithms / すべてのアルゴリズムに対し，より短く高速で*等価な*アルゴリズムが常に存在するというのが手抜きの際の仮定である
* Is this assumption always true? / この仮定は常に真か?
* I assume different languages take different time to solve problems / 問題解決の時間には言語間で差が生じると私は仮定する
* For practical problem solving there are always deadlines / 現実の問題解決には常に締切が存在する
* So different languages may solve or may not solve problems in a given time / 与えられた時間内で問題を解ける言語と解けない言語が存在し得る
* And different programming paradigms are practically not always equivalent with each other / 故に現実的には違うプログラミングパラダイム同士が等価とはいえない場合があり得る

### Shared-all .vs. shared-nothing programming paradigms

### Are references evil?

[TBD]
