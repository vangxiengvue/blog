---
description: ความน่าจะเป็น
---

# \[STA4\] Probability

ความน่าจะเป็นเนี่ย มันเป็นตัวเลขที่เอาไว้บอก**โอกาสการเกิดของเหตุการณ์**ที่เราตั้งขึ้นมา

เราเองก็น่าจะคุ้นชินกันมาแล้วแบบ "แก เรียนกับอาจารย์คนเนี้ยผ่านไม่ผ่านครึ่งๆ เลยนะ" หรืออาจจะแบบ "ชีวิตนี้ฉันคงจะหาแฟนไม่ได้แล้ว 😭"

แน่นอนว่า Statement พวกนี้เป็นการ**บ่งบอกถึงโอกาสการเกิด แต่ไม่ได้บอกนะว่ามันจะเกิดขึ้นจริงๆ** กับผู้พูดหรือผู้รับสารเอง \(ยกเว้นจะคำนวณออกมาแล้วได้ 0% หรือ 100% เอออันนี้ถึงจะไม่มีวันเกิดได้หรือเกิดขึ้นแน่ๆ\) ดังนั้นเวลาได้ยินใครเอา Statement แนวๆ นี้มาพูดใส่ ก็อย่าลืมใช้วิจารณญาณและสติของตัวเองในการพิจารณากันด้วยนะ \(เช่น นักศึกษาครึ่งหนึ่งอาจจะไม่ตั้งใจเรียนเองก็ได้ หรือ วันนี้หาแฟนไม่ได้ พรุ่งนี้อยู่ดีๆ อาจจะมีคนเข้ามาจีบก็ได้\)

หลักๆ แล้วความน่าจะเป็นมันจะมีวิธีการหาอยู่ 2 วิธีก็คือ:

1. การกำหนดความน่าจะเป็นโดยอาศัยตัวแบบของการทดลอง \(Experimental Model\)
2. การกำหนดความน่าจะเป็นโดยอาศัยผลจากการทดลอง \(Empirical Approach\)

เรามาเริ่มกันที่ตัวแรกกันก่อนเลย นั่นก็คือ…

## ความน่าจะเป็นโดยอาศัยตัวแบบของการทดลอง \(Experimental Model\)

{% hint style="info" %}
**นิยาม:** ในการทดลองเชิงสุ่ม ถ้าสามารถเขียน Sample Space ของผลลัพธ์โดยที่แต่ละผลลัพธ์มีโอกาสเกิดขึ้นได้เท่าๆ กัน และ $$A$$ เป็นเหตุการณ์ ความน่าจะเป็นของเหตุการณ์ $$A$$ เขียนแทนด้วย $$P(A)$$ จะได้ว่า

$$
P(A)=\frac{n(A)}{n(S)}
$$

โดยที่:

* $$n(A)$$ คือจำนวนสมาชิกของเหตุการณ์ $$A$$
* $$n(S)$$ คือจำนวนสมาชิกของ Sample Space
{% endhint %}

{% hint style="success" %}
**หมายเหตุ:** จะสังเกตว่าตัวนิยามจะใช้ $$n(X)$$ แทน $$|X|$$ \(เมื่อ $$X$$ เป็นเซต\) เพื่อบ่งบอกถึงจำนวนสมาชิกของเซต $$X$$ ซึ่งทั้งสอง notation สามารถใช้ได้เหมือนกัน แต่ในส่วนของผู้เขียนหลังจากนี้จะใช้เป็น $$n(X)$$ เพื่อให้สอดคล้องกับนิยามข้างต้น
{% endhint %}

วิธีเนี้ยจะเป็นวิธีการที่ใช้ในการออกสอบซะส่วนใหญ่ เพราะว่าวิธีนี้จะใช้วิธีการคำนวณเพียวๆ เลย ซึ่งอย่างที่นิยามบอก เราจะเอา**จำนวนสิ่งที่เกิดขึ้นได้ มาหารด้วยจำนวนสิ่งที่เกิดได้ทั้งหมด** ดังนั้นด้วยวิธีการนี้ เราจะได้เลขมาเพียวๆ สวยๆ เลย เดี๋ยวลองไปดูตัวอย่างกันดีกว่า

{% hint style="warning" %}
**ปัญหา 1:** จงหาความน่าจะเป็นที่นักศึกษา 7 คน จะเกิดคนละวันในวันของสัปดาห์
{% endhint %}

จากโจทย์ ข้อนี้จะมี S เป็น "นักศึกษา 7 คน เกิดวันต่างๆ ได้กี่รูปแบบ" เช่นอาจจะเป็น 'จ-อ-พ-พฤ-ศ-ส-อา' ก็ได้ หรืออาจจะเป็น 'จ-จ-จ-จ-จ-จ-จ' ก็ได้

เมื่อคำนวณออกมาก็จะได้ว่า $$n(S)=7\times7\times7\times7\times7\times7\times7=7^7$$

ต่อมา เราก็กำหนดเหตุการณ์ขึ้นมาแทนสิ่งที่เราสนใจ \(ก็คือโจทย์นั่นเอง\) ก็คือ "กำหนดให้ A แทนเหตุการณ์ที่นักศึกษา 7 คน เกิดคนละวันในวันของสัปดาห์"

วิธีการคิดคือ ให้คิดว่านักศึกษาคนแรกเลือกมา 1 วันจาก 7 วัน ก็จะเหลือให้คนที่สองเลือก 1 วันจาก 6 วัน ทำอย่างนี้ไปเรื่อยๆ จนกระทั่งคนสุดท้ายจะเหลือให้เลือก 1 วัน เท่านี้ทั้ง 7 คนก็จะได้วันที่ไม่ซ้ำกันแล้ว

จะได้ว่า $$n(A)=7\times6\times5\times4\times3\times2\times1=7!$$

ดังนั้น เราก็จะสามารถคำนวณหาความน่าจะเป็นของเหตุการณ์ A ได้ว่า

$$
P(A)=\frac{n(A)}{n(S)}=\frac{7!}{7^7}
$$

**ดังนั้น:** ความน่าจะเป็นที่นักศึกษา 7 คน จะเกิดคนละวันในวันของสัปดาห์ คือ $$\frac{7!}{7^7}$$

จะเห็นว่า วิธีการนี้ค่อนข้างเหมาะสมกับการคำนวณมากๆ ได้ค่าดูดีมีเหตุผล แต่วิธีการนี้จริงๆ แล้วมีข้อเสียอยู่ 2 ข้อก็คือ:

1. **Sample Space ต้องเป็นเซตจำกัด:** เหตุการณ์บางอย่างสามารถมี Sample Space เป็นอนันต์ได้หรือสามารถหา Sample Space ได้ยาก ซึ่งถ้าเราหา Sample Space ไม่ได้ เราก็หาความน่าจะเป็นของมันด้วยวิธีข้างต้นไม่ได้
2. **ผลลัพธ์จากการทดลองแต่ละผลลัพธ์ต้องมีโอกาสเกิดขึ้นได้เท่าๆ กัน:** เช่น เราอาจจะบอกได้ว่าลูกเต๋าที่มี 6 หน้า จะมีโอกาสออกแต่ละหน้าเท่าๆ กัน แต่ถ้าสมมติว่าเราใช้ลูกเต๋าบิ่นที่มีหน้าหน้าหนึ่งมีโอกาสออกได้เป็น 2 เท่าของหน้าอื่น เราจะใช้วิธีคิดแบบนี้ไม่ได้

ถ้าเราเจอปัญหาทั้ง 2 ข้อด้านบน เราก็อาจจะต้องปรับวิธีการคำนวณ หรือเราสามารถใช้ได้อีกวิธีนั่นก็คือ…

## ความน่าจะเป็นโดยอาศัยผลจากการทดลอง \(Empirical Approach\)

{% hint style="info" %}
**นิยาม:** ในการทดลองเชิงสุ่ม $$n$$ ครั้ง เกิดเหตุการณ์ที่ต้องการ $$S$$ ครั้ง ถ้า $$n$$ มีค่ามากพอ เรากล่าวได้ว่าความน่าจะเป็นที่จะได้เหตุการณ์ที่ต้องการในการทดลองแต่ละครั้งจะมีค่าเป็น $$p=\frac{S}{n}$$ และความน่าจะเป็นที่จะได้เหตุการณ์ที่ไม่ต้องการจะเท่ากับ $$q=\frac{n-S}{n}$$
{% endhint %}

พูดให้ง่ายขึ้นอีก ก็คือ **อยากรู้ก็ลองทำดูสิ**

ฮะ? ลองทำ? ยังไงหรอ 🤨?

หลักการของวิธีนี้ก็ตามที่บอกเลยคือ เราก็ทดลองไปเรื่อยๆ แล้วจดบันทึก 2 อย่างคือ:

1. ทำไปแล้วกี่ครั้ง \(n\)
2. ได้ตามที่อยากได้แล้วกี่ครั้ง \(S\)

พอเราบันทึกค่าทั้ง 2 อย่างนี้ได้ ก็เอามาคำนวณด้วยสูตร $$p=\frac{S}{n}$$ เราก็จะได้ความน่าจะเป็นออกมา

เอาเป็นว่าเราไปลองดูตัวอย่างง่ายๆ กันดีกว่า

{% hint style="warning" %}
**ปัญหา 1:** เด็กชายคนหนึ่งอยากรู้ว่าตนเองนั้นเล่นเกมเกมหนึ่งเก่งแค่ไหน จึงทำการทดลองเล่นเกมติดต่อกัน 20 ตา ผลปรากฏว่าเล่นชนะไปทั้งหมด 12 ตา แพ้ 8 ตา เด็กชายคนนี้มีความน่าจะเป็นที่จะเล่นเกมนี้ชนะเป็นเท่าไร?
{% endhint %}

อ่านโจทย์กันเสร็จแล้วก็น่าจะตอบกันในใจได้เลยใช่มะ? เพราะถ้าเล่น 20 ตา ชนะ 12 ก็แสดงว่ามีความน่าจะเป็นในการชนะ $$\frac{12}{20}$$ สิ?

ถูกต้องแล้วจ้า และนั่นก็คือคอนเซปต์ของวิธีการนี้เลย เป็นเพราะเนื่องจากเราไม่รู้ว่า เราจะแพ้ชนะในรูปแบบไหน เราก็เลยทดลองเล่นมันซะเลย

**ดังนั้น:** เด็กชายคนนี้มีความน่าจะเป็นที่จะเล่นเกมนี้ชนะเป็น $$\frac{12}{20}=\frac{3}{5}$$

เราน่าจะพอเห็นข้อเสียของวิธีนี้กันเนอะ นั่นก็คือ ค่าที่ได้อาจจะไม่ตรงกับความจริงก็ได้ \(เช่น เล่นเกมชนะ 12 ตาเพราะอาจจะเจอทีมฝั่งตรงข้ามเล่นไม่ดีก็ได้\) ดังนั้นวิธีนี้**ต้องทำการทดลองมากพอที่จะสามารถสรุปได้**

ทั้งสองวิธีที่เราได้พูดถึงไปล้วนแล้วเป็นวิธีหาความน่าจะเป็นของเหตุการณ์ต่างๆ ที่จะเกิดขึ้น เดี๋ยวจะขอตัดเนื้อหาไว้แต่เพียงตรงนี้ก่อน แล้วเดี๋ยว EP หน้าเรามาดูเนื้อหาในเรื่องของสมบัติความน่าจะเป็นกัน  เอาเป็นว่า เราไปดูสรุปสำหรับ EP นี้กันเลย

## สรุปเนื้อหา

* ความน่าจะเป็น
  * คือเลขในช่วง \[0,1\] ที่บอกว่ามีโอกาสการเกิดเหตุการณ์ได้เท่าไร
  * $$P(A)=\frac{n(A)}{n(S)}$$ **"ความน่าจะเป็นของ A = A เกิดได้กี่แบบ / ทั้งหมดเกิดได้กี่แบบ"**
  * **ตัวอย่าง:** โยนลูกเต๋า 1 ลูก ความน่าจะเป็นที่จะออก 5 หรือ 6 เป็นเท่าไร?
    * วิธีที่ 1: คำนวณจาก Sample Space
      * จะได้ว่า: $$P(โยนลูกเต๋าออก\ 5, 6)=\frac{n(\{5,6\})}{n(\{1,2,3,4,5,6\})}=\frac{2}{6}=\frac{1}{3}$$
      * เรียกวิธีนี้ว่า "อาศัยตัวแบบของการทดลอง"
      * ข้อเสีย:
        * S ต้องนับได้ \(เพราะเราต้องใช้ S คำนวณ\)
        * ผลลัพธ์แต่ละผลลัพธ์ \(ของเหตุการณ์\) ต้องมีความน่าจะเป็นเท่ากัน \(ถ้ามีบางผลลัพธ์เกิดได้มาก/น้อยกว่าตัวอื่น จะต้องปรับการคำนวณหรือใช้วิธีอื่น\)
    * วิธีที่ 2: โยนลูกเต๋าไปเรื่อยๆ สัก 1,000 ครั้ง แล้วจดไว้ว่าออกเลข 5 กับ 6 กี่ครั้ง \(สมมติว่าโยน 1000 ครั้ง ออกเลข 5 กับ 6 ทั้งหมด 333 ครั้ง\)
      * จะได้ว่า: $$P=\frac{S}{n}=\frac{333}{1000}\approx\frac{1}{3}$$
      * เรียกวิธีนี้ว่า "อาศัยผลจากการทดลอง"
      * ข้อเสีย: ต้องทดลองไปเรื่อยๆ จนจำนวนครั้งมากพอ จึงจะสามารถสรุปได้

