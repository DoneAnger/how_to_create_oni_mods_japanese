# Stinky

AIを定義、設定する場所を探しているときに偶然みつけた

***
    [SkipSaveFileSerialization]
    public class Stinky : StateMachineComponent<Stinky.StatesInstance>
    {
        .........
			MinionIdentity minionIdentity = liveMinionIdentities[i];
			if (minionIdentity.gameObject != gameObject.gameObject)
			{
				Vector2 b = minionIdentity.transform.GetPosition();
				float num = Vector2.SqrMagnitude(a - b);
				if (num <= 2.25f)
				{
					minionIdentity.Trigger(508119890, Strings.Get("STRINGS.DUPLICANTS.DISEASES.PUTRIDODOUR.CRINGE_EFFECT").String);
					minionIdentity.GetComponent<Effects>().Add("SmelledStinky", true);
					minionIdentity.gameObject.GetSMI<ThoughtGraph.Instance>().AddThought(Db.Get().Thoughts.PutridOdour);
				}
			}
***

スティンキーマシーンコンポーネントというものにスティンキーの匂いを追加するメソッド

スティンキーへの愛が感じられる
