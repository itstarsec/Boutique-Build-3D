Tôi đính kèm HoanNguyen_Boutique_v13_Full_Source.zip. Hãy dùng chính source trong ZIP để khôi phục website hiện tại với toàn bộ chức năng và giao diện đã có. Đây là yêu cầu thực thi, không phải tạo ý tưởng hoặc viết một demo mới.

Vai trò và nguồn chuẩn

Đóng vai Senior Full-Stack Engineer, Three.js Engineer và kiến trúc sư boutique hospitality. Đọc các tệp trong gói trước khi thao tác:

BAT_DAU_O_DAY.md, RESTORE_GUIDE.md, FEATURE_PARITY.md.

SOURCE_PROVENANCE.json; chạy python tools/verify-package.py hoặc tự kiểm tra toàn bộ SHA256 bằng công cụ tương đương.

source/package.json, source/package-lock.json, source/vite.config.ts, source/tsconfig.json, source/.openai/hosting.json.

source/src/App.tsx, src/main.tsx, engine/model/store/storage/usePersistence/export và các component 2D/3D/Journey/Designer.

Toàn bộ source/src/experience/, ba manifest GLB, authoring A/B/vận hành và source/docs/all-spaces-delivery-20261031.md.

source/public/integration-notes.md, các giấy phép và PDF gốc 14 trang ở blueprint/. Nếu sửa thiết kế phải xem đủ ảnh và sơ đồ PDF, không chỉ dựa vào tóm tắt.

Bản chuẩn: Sites version 13, commit ccf50ef6b8a8b83fc3ca41c6f1567cea9c1ab78e.
Site ID: appgprj_6ad435d408188191a8f4c609acd9e0de.
URL gốc: https://co-thach-boutique-retreat.exactlamp6.chatgpt.site/.
Quyền truy cập được xác nhận tại thời điểm xuất: public. Phải đọc quyền hiện tại bằng Sites trước mọi triển khai sau này; không tự đổi quyền.

Source và gói build là nguồn chuẩn cho hành vi hiện có. Prompt là tài liệu bàn giao, không thay thế code. Những báo cáo phase cũ có thể ghi số liệu cũ; ưu tiên báo cáo v13 và manifest hiện tại.

Phạm vi triển khai

Trước tiên giải nén và khôi phục tại workspace, chạy kiểm tra. Không tạo Site mới hoặc thay website đang chạy chỉ để chứng minh khôi phục thành công.

Khi tôi yêu cầu cập nhật website gốc: dùng Sites để mở đúng project_id, kiểm tra source/live version hiện tại, tạo baseline và tích hợp bản cần khôi phục; không tự ghi đè những thay đổi mới hơn v13. Giữ domain, audience, schema và dữ liệu. Dùng quy trình mở source, build, push, save và deploy của skill Sites đang cài; không tự chế credential hoặc dùng credential trong lịch sử.

Nếu tôi yêu cầu rõ một Site độc lập: dùng một thư mục template đã làm sạch identity, Git và runtime; bỏ project_id của Site gốc trong bản sao trước khi đăng ký Site mới. Không đổi identity hoặc triển khai nhầm lên Site gốc. Site mới dùng quyền riêng tư mặc định trừ khi tôi yêu cầu khác.

Nếu yêu cầu chỉ khôi phục hoặc kiểm tra local: không xuất bản.

Không được thay thế hoặc làm mất

Không viết lại từ đầu, chuyển framework, rút gọn thành landing page, dùng template khác hoặc tạo iframe dẫn sang demo.

Không bỏ các thành phần chỉ vì code dài. Không làm lại 3D bằng ảnh phẳng/panorama/video/parallax.

Không dùng bản 12 bungalow làm mặc định. Mẫu 12 bungalow chỉ là phương án lịch sử được bảo toàn.

Không tự thêm hồ bơi, nhà hàng lớn, phòng nghỉ thứ bảy, dịch vụ đặt phòng/thu tiền/khóa số thật hoặc công trình không có trong dữ liệu.

Không sửa dữ liệu cá nhân bằng seed mặc định. Không reset IndexedDB hoặc đổi khóa lưu để che lỗi.

Không nâng dependency hoặc đổi texture/font/model nếu chưa có lỗi cụ thể yêu cầu sửa. Giữ MIT/CC0/OFL và nguồn ảnh từ PDF.

Không mặc định mọi báo cáo kiểm tra CPU là ảnh WebGL, Blender render hoặc chứng nhận điện thoại thật.

Bản sắc và chương trình kiến trúc phải giữ

HOÀN NGUYÊN BOUTIQUE — Vườn hiên Cổ Thạch.
“Một khoảng hiên để trở về.”

Nhỏ, ấm, có chiều sâu. Vữa trắng ấm, sắc đất, gỗ/đá/linen, vòm ở cổng/hiên, mái cách nhiệt giấu kín, vườn sỏi khô chịu hạn. Giữ nguyên header/footer, typography tiếng Việt, bố cục hồ sơ kiến trúc, ảnh, chuyển cảnh nhẹ, closeup và mobile UI.

Hai dãy, mỗi dãy 2A + 1B là bố trí đề xuất: A01/A02/B03, A04/A05/B06.

A trong tường 3,20 × 5,25 m; B 3,80 × 5,25 m; cao 3 m; hiên 1,45 m; tường mặc định 0,10 m.

Cụm vận hành trong tường 6,80 × 3,80 m, ngoài tường 7 × 4 m = 28 m².

Giữ phần đất phía sau, ba luồng khách / buồng phòng-kỹ thuật / thi công giai đoạn sau.

Khung 60 × 80 m là tham chiếu chưa xác nhận diện tích đất thực. Không tự gán ranh địa chính hoặc tọa độ. Không ép chỉ tiêu 4,1% / 18–22% / ≥75% thành biểu đồ đất cộng 100%.

“Hồ sơ ý tưởng • Chưa dùng để thi công”. Ngân sách PDF 885 + 95 = 980 triệu và kế hoạch 22 tuần giữ nguyên nguồn/chú thích.

Chức năng bắt buộc giữ nguyên

Trải nghiệm chính và quy hoạch

Câu chuyện / Vườn hiên / Hai kiểu phòng / Phương án; chuyến dạo cổng–vườn–hiên–phòng; bốn góc cận có chủ đích; chọn phòng, bật/tắt mái, ánh sáng, luồng và lớp đất dự trữ. Tesla Roadster là đạo cụ hình khối minh họa ở bãi xe, không phải tài sản/dịch vụ có thật.

2D SVG và 3D dùng chung dữ liệu công trình. Giữ chọn/di chuyển/xoay/nhân bản/xóa, thay tên/kích thước/chiều cao/vật liệu, pan/zoom/grid/snap/thước/lớp theo implementation hiện có, undo/redo, cảnh báo chồng lấn/vượt ranh, bảng diện tích/khối lượng/đơn giá, CSV/JSON/PNG và in PDF. Không gộp trùng hiên/mặt nước/cảnh quan/phần chiếm đất. Source mm, scene m; không đổi quy ước.

Chi tiết nội thất toàn dự án

Giữ mục “Bước vào từng không gian”, entry Journey “Nội thất & WC”, CTA phòng mẫu và dropdown chuyển đủ bảy không gian. Chỉ một canvas chi tiết hoạt động; viewer nền dùng 2D khi overlay mở.

Ba template GLB thật đã có:

A: /assets/interior/room-a.glb, 756.020 byte, 22.371 tam giác.

B: /assets/interior/room-b.glb, 804.300 byte, 24.243 tam giác.

Vận hành: /assets/interior/operations.glb, 433.732 byte, 11.164 tam giác.

Bốn phòng A dùng template A; hai B dùng B có daybed. Các bản chỉnh được dựng procedural theo thông số trong phạm vi supportsRoom. Không dùng GLB mẫu để âm thầm bỏ qua chỉnh sửa của người dùng.

Cả sáu phòng có geometry thật cho shell, giường/linen/đèn/tủ/ghế/hiên, cửa kính/rèm, bồn cầu sứ rỗng, lavabo/tủ/gương, sen/vách kính, phụ kiện và cửa WC trượt riêng. WC A khoảng 4,80 m²; B 5,70 m², nằm trong diện tích hiện hữu.

Cụm vận hành có quầy nhận phòng, bữa sáng nhẹ, máy giặt/sấy, kệ đồ vải, đầu mối kỹ thuật và WC nhân viên với toilet/lavabo/gương. WC nhân viên ~3 m² là chi tiết đề xuất bên trong 28 m², không có vòi tắm. Nhãn diện tích trong vỏ nhà chưa trừ vách ngăn đề xuất phải giữ đúng. Không tự nhận hệ nhận phòng, máy giặt, van/tủ điện là tích hợp thiết bị thật.

Giữ Guided/Free Walk, camera waypoint, WASD/Shift/chuột/pointer lock, joystick/chạm, reset/exit; capsule collision theo sàn, tường, nội thất, kính, vùng biên và hai trạng thái cửa; không xuyên đồ hoặc xuyên tường trên tuyến dẫn hướng. Giữ các hotspot gắn object, vật liệu gỗ chuẩn bị sẵn, mở/khép rèm ở phòng khách, ba chế độ sáng tác động lên đèn thật. Gương gần đúng; không có mô phỏng nước/xả bồn cầu, GI bake hoặc nghiên cứu nắng theo địa điểm.

Lưu trữ và hiệu năng

IndexedDB co-thach-retreat-v1, projects/versions; hn-current-v2, hn-version:*, hn-archive:*; giữ nguyên current/versions của bản cũ. Tự lưu có trạng thái, khôi phục sau reload, xử lý xung đột tab, kho phương án, schema validation khi nhập JSON.

Giữ lazy import, chỉ fetch template được chọn, cache theo template, xác minh manifest/hash, timeout/retry, hủy fetch/texture/GPU khi đóng/đổi cảnh. Texture sidecar CC0 tối đa 512 px, quality tiers và Lite, reduced-motion, pause offscreen/hidden tab, touch-cancel sạch, safe-area, fallback ảnh/sơ đồ khi WebGL lỗi. Không yêu cầu Blender để chạy runtime.

Trình tự thực thi

Đối chiếu ZIP, checksum, snapshot và identity. Báo tệp thiếu/hỏng, không tự thay bằng placeholder.

Dùng nguyên source/. Cài dependency theo lockfile bằng helper của môi trường Sites khi phù hợp hoặc npm ci; ưu tiên Node 24.x, đã kiểm tra Node 24.22.1 / npm 11.9.0.

Chạy npm test, npm run build. Baseline là 84/84 test. Nếu lỗi, chẩn đoán và sửa đúng nguyên nhân, không xóa test hay hạ yêu cầu để pass.

Có thể xem ngay prebuilt/dist bằng node tools/serve-prebuilt.mjs ở môi trường local thông thường. Trong môi trường Sites managed phải tuân thủ cơ chế preview của skill Sites, không tự mở server thay thế hoặc vượt hạn chế browser.

Dùng FEATURE_PARITY.md để kiểm tra các CTA, editor, lưu/tải, JSON/CSV/PNG, cả bảy scene, camera/door/collision/hotspot/light/fallback và mobile UI.

Mọi dữ liệu riêng cần file JSON từ trình duyệt cũ do tôi cung cấp. Dữ liệu mẫu trong ZIP không phải bản sao dữ liệu cá nhân. Không tự tuyên bố đã khôi phục IndexedDB của máy khác.

Chỉ triển khai khi phạm vi yêu cầu đã cho phép; dùng đúng Site/audience, package dist theo skill Sites và chờ kết quả native trả thành công. Không đổi URL tùy ý.

Báo rõ source/asset đã khôi phục, test/build đã chạy, URL nếu có, những điều chưa kiểm chứng. Không nói “100% mọi thiết bị” khi chưa đo thực tế.

Giới hạn đã biết phải giữ trung thực

84 test là kiểm tra source/SSR/geometry/lifecycle, không phải toàn bộ tương tác live trên thiết bị. Các góc render trong docs là CPU triangle/albedo diagnostics, không phải native Blender/WebGL/PBR/GI attestation. Trước khi xuất, browser GPU/iPhone Safari/Android Chrome thật, FPS và Lighthouse chưa được nghiệm thu đầy đủ; lần preview gần nhất bị chặn do hạn mức. Có một cảnh báo chunk Three/LeanScene lớn; đừng che warning để tuyên bố tối ưu.

Không cần dịch vụ img2interior hoặc Blender để dùng website hiện có. Pipeline tham khảo img2threejs đã được nghiên cứu nhưng Blender/bpy, neural reconstruction và native bake chưa chạy. Đừng tạo ảnh/video rồi gọi là interactive geometry.

Mục tiêu cuối: khôi phục bản Hoàn Nguyên v13 bằng chính source được cung cấp, giữ nguyên đầy đủ hành vi và giao diện, làm cho người xem thực sự bước vào cả phòng nghỉ lẫn WC và cụm vận hành, trong đúng phạm vi kiểm chứng và dữ liệu có thật.
