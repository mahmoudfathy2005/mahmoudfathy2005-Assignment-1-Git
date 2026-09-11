1. git squash

الـ Squash معناه إني أدمج كذا Commit في Commit واحدة.

مثال: لو عملت كذا Commit وأنا بعمل Feature، أقدر أدمجهم في Commit واحدة عشان الـ History يبقى أنضف.

2. git merge vs git rebase

Merge: بستخدمه عشان أدمج Branch في Branch تاني.

git merge feature/login

Rebase: بستخدمه عشان أحدث الـ Branch بتاعي بآخر تغييرات من Branch تاني.

git rebase main

ببساطة: Merge بيحافظ على الـ History، وRebase بيخليه أبسط.

3. git help

بستخدمه لما أنسى طريقة استخدام أمر معين.

git help merge

بيطلعلي شرح الأمر والـ Options بتاعته.

4. git cherry-pick

بستخدمه عشان أنقل Commit معينة من Branch لBranch تاني.

مثال: عندي Bug Fix في Branch تاني وعايز الـ Fix ده بس، من غير ما أعمل Merge للـ Branch كله.

5. git clean

بستخدمه عشان أمسح الملفات اللي Git مش متابعها.

مثال: عندي ملفات مؤقتة ومش محتاجها.

git clean -n

الأمر ده بيوريني الملفات اللي ممكن تتمسح.

6. git grep

بستخدمه عشان أبحث عن كلمة أو Code داخل المشروع.

git grep "UserManager"

مثلاً لو عايز أعرف UserManager مستخدم فين.

7. git blame

بستخدمه عشان أعرف مين عدّل سطر معين في الكود.

git blame Program.cs

مفيد لو لقيت سطر ومش عارف مين اللي غيره.

8. git bisect

بستخدمه لما يكون عندي Bug ومش عارف أنهي Commit عملت المشكلة.

Git بيساعدني أدوّر بين الـ Commits لحد ما أوصل للـ Commit اللي فيها المشكلة.

9. git shortlog

بستخدمه عشان أشوف ملخص عن الـ Commits والناس اللي اشتغلت على المشروع.

git shortlog -sn

ممكن أعرف كل شخص عمل كام Commit.

10. git prune

بستخدمه لتنظيف الـ Repository من Objects قديمة ومش مستخدمة.

مش بستخدمه كتير، وبيكون مفيد في تنظيف الـ Repository.

11. git worktree

بستخدمه عشان أشتغل على أكتر من Branch في نفس الوقت.

مثال: أنا شغال على Feature وفجأة محتاج أصلح Bug، أقدر أعمل Worktree للـ Bug من غير ما أوقف شغلي الحالي.

12. git verify-commit

بستخدمه عشان أتأكد إن الـ Commit عليها Signature صحيحة.

git verify-commit <commit-hash>

مفيد في المشاريع اللي بتهتم بأمان الـ Commits.

13. git filter-repo

بستخدمه لو عايز أشيل ملف من تاريخ المشروع كله.

مثال: لو بالغلط رفعت Password أو API Key، أقدر أستخدمه عشان أشيل الملف من الـ History.

git filter-repo --path secret.txt --invert-paths

لازم أستخدمه بحذر لأنه بيغير الـ History.
