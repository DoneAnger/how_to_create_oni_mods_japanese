# Mod作成超メモ

ぱさらんドキュメントに書いてない部分の調査を超メモ的にまとめる

ワークショップのModsからいろいろ読み取る
サンプルとしていろいろ作ってる方のgithub
https://github.com/peterhaneve/ONIMods

PLibのReadMeに最初に読み込まれそうな関数発見

***
    public static class Mod_OnLoad
    {
        public static void OnLoad()
        {
            PLib.PUtil.LogModInit();
            PLib.POptions.RegisterOptions(typeof(TestModSetting));
        }
    }
***
