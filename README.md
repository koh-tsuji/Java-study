# Java-study

Java学習記録

2026/06/09
・Eclipse導入
・scanner
・if文
・GitHub導入

2026/06/10
・GitHub登録
・新しいリポジトリ作成
Eclipseで作成した成果を保存していく。
次回：While文

2026/06/14
・while文振り返り
・for文振り返り
次回：配列（Array）

2026/06/15
・配列Array振り返り
・配列×for文
・配列の長さを取得する⇒scores.length
・合計値の求め方sum
次回：平均値、最大値、最小値

2026/06/16
・平均値average⇒double average = (double) sum / numbers.length;
・最大値max⇒if (numbers[i] > max)
・最小値min⇒if (numbers[i] < min)
次回：メソッド

2026/06/17
・引数と戻り値のあるメゾット⇒public static int subtract(int a, int b) { return a - b；}
・掛け算メゾット⇒public static int multiply(int a, int b) { return a * b;}
・booleanを返すメゾット⇒public static boolean isAdult(int age) { return(int age >= 18); }
・配列＋for文＋return⇒public static int sumArray(int[] numbers) {～～
次回：配列の平均値を返すメゾットaverageArray

2026/06/19
・averageArray⇒public static double averageArray(int [] numbers){
・maxArray⇒public static int maxArray(int [] numbers) {
・minArray⇒public static int minArray(int [] numbers) {
・人数カウントの数え方⇒public static int countAdults(int [] ages) {
次回：クラス、オブジェクト

2026/6/21
・クラス⇒class Person：Personという新しい型を作る
・オブジェクト⇒Person person ＝ new Person();　：Person型のオブジェクトを作る
・フィールド⇒Person.name ="田中 "; ：オブジェクトの場所を保存する場所
・インスタンスメゾット⇒public void ～　System.out.println(＊＊)　：オブジェクトがもつ処理
・コンストラクタ⇒Person(int ○○,String ×× )｛
　　　　　　　　　　　this.○○ = ○○;
                    this.×× = ××;
                ：オブジェクト作成時に初期値を設定する仕組み
・this⇒this.○○ = ○○;　：左はフィールド、右は引数
          
2026/06/24
・タスクアプリ制作に挑戦
⇒
★while文を学習
　・追加したコード
　　while (choice != 3) {
　　...}
・学んだこと
・!=⇒等しくない
つまり、while (choice != 3)は
choice が 3 と等しくない間は繰り返すという意味。
・変数の更新を理解
　choice = scanner.nextInt();を毎回実行することで、
　入力⇒choiceに保存⇒while条件を再判定していることを学んだ。
・Scannerの位置を修正
　最初はscanner.close();が while の中にあった。
　その結果
　1回入力⇒Scanner終了⇒次の入力ができない。
　修正後：while (...) {...}
　scanner.close();　に変更。
・入力チェック機能を追加
　追加したコード
if (choice < 1 || choice > 3) {
    System.out.println("1から3を入力して下さい");
}
・学んだこと
　「||」は、またはという意味
 次回：ArrayListでタスク追加

 2026/06/25
・String学習
・nextLine()で文字入力
・tasks.add()でタスク保存

★現在できること
・メニュー表示
・タスク入力
・ArrayListへ保存

次回：タスク一覧表示

