# รีวิว: KRU-OFFY/Claude-Project-CreatorOS-AI (2026-11-10)

ผล: 🟡 ไม่ติดตั้ง เก็บแค่ไอเดีย Compliance ไทย

## แก่นคืออะไร
เว็บแอปเต็มระบบ (Next.js 15 + Supabase + Vercel) ไม่ใช่ Skill: เลือกสินค้า → AI เขียนคอนเทนต์ → ตรวจกฎโฆษณา → ตั้งเวลาโพสต์ → Analytics → AI Advisor, 11 หน้า, ทีมหลาย role. repo มี commit เดียว (12 ก.ค. 2026)

## ประโยชน์จริง
- ชุดกฎ Compliance ไทยแยกหมวด (เครื่องสำอาง, อาหารเสริม/อย., การเงิน)
- สูตรให้คะแนนสินค้า (hero ≥80 / growth ≥60 / test ≥40)

## ข้อเสีย / กับดัก
- ต้องสมัคร/ใช้ key: Supabase, Vercel (cron ทุก 5 นาทีต้อง Pro), Meta/TikTok/Google OAuth, Anthropic, render worker แยก
- Shopee Video / Shopee Live / Lemon8 / X เป็น stub (copy-to-post)
- ไม่มีไฟล์ LICENSE: คัดลอกโค้ดไม่ได้ ใช้ได้แค่ไอเดีย
- ซ้อนกับโน้ตใน vault: Affiliate-AI-Shopee-Engine, Shopee-Content-Studio, TXT-Affiliate-Distributor

## ที่ทำ (Boss เลือก A)
เขียน Skill `thai-ad-compliance-check` ใหม่เอง (ไม่ก๊อปโค้ด) ดู `skills/thai-ad-compliance-check/SKILL.md`
ติดตั้งแล้วที่ `~/.agents/skills/thai-ad-compliance-check/` และต่อ Delta ในโน้ต vault Affiliate-AI-Shopee-Engine.md

## ยังไม่ได้ทำ
- ทดสอบเรียกใช้กับสคริปต์ตัวอย่าง
- คัดลอกไป `~/.claude/skills` (Claude Code)
