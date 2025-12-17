<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>So Sánh Giải Pháp MDM: Mosyle - JumpCloud - Iru</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; }
        .tab-active { border-bottom: 2px solid #2563eb; color: #2563eb; font-weight: 600; }
        .tab-inactive { color: #6b7280; }
        .tab-inactive:hover { color: #374151; }
    </style>
</head>
<body class="bg-gray-50 min-h-screen">

    <!-- Header -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <i class="fa-solid fa-layer-group text-blue-600 text-2xl"></i>
                <h1 class="text-xl font-bold text-gray-900">So Sánh MDM Dashboard</h1>
            </div>
            <div class="text-sm text-gray-500 hidden sm:block">
                Dữ liệu cập nhật: Mosyle, JumpCloud, Iru
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
        
        <!-- Tabs Navigation -->
        <div class="border-b border-gray-200 mb-6">
            <nav class="-mb-px flex space-x-8" aria-label="Tabs">
                <button onclick="switchTab('overview')" id="tab-overview" class="tab-active whitespace-nowrap py-4 px-1 border-b-2 font-medium text-sm">
                    <i class="fa-solid fa-table-columns mr-2"></i>Tổng Quan & Bảo Mật
                </button>
                <button onclick="switchTab('pricing')" id="tab-pricing" class="tab-inactive whitespace-nowrap py-4 px-1 border-b-2 border-transparent font-medium text-sm">
                    <i class="fa-solid fa-tags mr-2"></i>Giá Cả & Chính Sách
                </button>
                <button onclick="switchTab('recommendation')" id="tab-recommendation" class="tab-inactive whitespace-nowrap py-4 px-1 border-b-2 border-transparent font-medium text-sm">
                    <i class="fa-solid fa-lightbulb mr-2"></i>Lời Khuyên & Ví Von
                </button>
            </nav>
        </div>

        <!-- TAB 1: OVERVIEW & SECURITY -->
        <div id="content-overview" class="space-y-6 animate-fade-in">
            <!-- Intro Cards -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Mosyle -->
                <div class="bg-white rounded-xl shadow-sm border border-indigo-100 p-6 relative overflow-hidden group hover:shadow-md transition">
                    <div class="absolute top-0 right-0 p-4 opacity-10 group-hover:opacity-20 transition">
                        <i class="fa-brands fa-apple text-6xl text-indigo-600"></i>
                    </div>
                    <div class="flex items-center mb-4">
                        <div class="h-10 w-10 rounded-full bg-indigo-100 flex items-center justify-center text-indigo-600 font-bold mr-3">M</div>
                        <h2 class="text-lg font-bold text-gray-900">Mosyle</h2>
                    </div>
                    <p class="text-gray-600 text-sm mb-4 h-10">Chuyên gia hệ sinh thái Apple với khả năng triển khai Zero-Touch.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2 py-1 bg-indigo-50 text-indigo-700 text-xs rounded-full border border-indigo-200">Apple Only</span>
                        <span class="px-2 py-1 bg-green-50 text-green-700 text-xs rounded-full border border-green-200">Giá tốt nhất</span>
                    </div>
                </div>

                <!-- JumpCloud -->
                <div class="bg-white rounded-xl shadow-sm border border-orange-100 p-6 relative overflow-hidden group hover:shadow-md transition">
                    <div class="absolute top-0 right-0 p-4 opacity-10 group-hover:opacity-20 transition">
                        <i class="fa-solid fa-id-card text-6xl text-orange-600"></i>
                    </div>
                    <div class="flex items-center mb-4">
                        <div class="h-10 w-10 rounded-full bg-orange-100 flex items-center justify-center text-orange-600 font-bold mr-3">J</div>
                        <h2 class="text-lg font-bold text-gray-900">JumpCloud</h2>
                    </div>
                    <p class="text-gray-600 text-sm mb-4 h-10">Nền tảng mở (Open Directory) kết hợp quản lý thiết bị và danh tính.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2 py-1 bg-gray-100 text-gray-700 text-xs rounded-full border border-gray-200">Đa nền tảng</span>
                        <span class="px-2 py-1 bg-orange-50 text-orange-700 text-xs rounded-full border border-orange-200">Identity Focus</span>
                    </div>
                </div>

                <!-- Iru -->
                <div class="bg-white rounded-xl shadow-sm border border-purple-100 p-6 relative overflow-hidden group hover:shadow-md transition">
                    <div class="absolute top-0 right-0 p-4 opacity-10 group-hover:opacity-20 transition">
                        <i class="fa-solid fa-robot text-6xl text-purple-600"></i>
                    </div>
                    <div class="flex items-center mb-4">
                        <div class="h-10 w-10 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 font-bold mr-3">I</div>
                        <h2 class="text-lg font-bold text-gray-900">Iru (Kandji)</h2>
                    </div>
                    <p class="text-gray-600 text-sm mb-4 h-10">Quản lý thống nhất được hỗ trợ bởi AI và tự động hóa tuân thủ.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2 py-1 bg-gray-100 text-gray-700 text-xs rounded-full border border-gray-200">Đa nền tảng</span>
                        <span class="px-2 py-1 bg-purple-50 text-purple-700 text-xs rounded-full border border-purple-200">AI Driven</span>
                    </div>
                </div>
            </div>

            <!-- Comparison Table -->
            <div class="bg-white rounded-xl shadow-sm overflow-hidden border border-gray-200">
                <div class="px-6 py-4 border-b border-gray-200 bg-gray-50">
                    <h3 class="font-semibold text-gray-800">So Sánh Chi Tiết: Bảo Mật & Hệ Sinh Thái</h3>
                </div>
                <div class="overflow-x-auto">
                    <table class="min-w-full divide-y divide-gray-200">
                        <thead class="bg-gray-50">
                            <tr>
                                <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Tiêu chí</th>
                                <th scope="col" class="px-6 py-3 text-left text-xs font-bold text-indigo-700 uppercase tracking-wider bg-indigo-50/50">Mosyle</th>
                                <th scope="col" class="px-6 py-3 text-left text-xs font-bold text-orange-700 uppercase tracking-wider bg-orange-50/50">JumpCloud</th>
                                <th scope="col" class="px-6 py-3 text-left text-xs font-bold text-purple-700 uppercase tracking-wider bg-purple-50/50">Iru</th>
                            </tr>
                        </thead>
                        <tbody class="bg-white divide-y divide-gray-200 text-sm">
                            <tr>
                                <td class="px-6 py-4 font-medium text-gray-900">Hệ sinh thái hỗ trợ</td>
                                <td class="px-6 py-4 text-gray-600">
                                    <i class="fa-brands fa-apple mr-1"></i> Apple Only<br>
                                    <span class="text-xs text-gray-500">(macOS, iOS, iPadOS, tvOS...)</span>
                                </td>
                                <td class="px-6 py-4 text-gray-600">
                                    <i class="fa-solid fa-layer-group mr-1"></i> Đa nền tảng<br>
                                    <span class="text-xs text-gray-500">(Win, Mac, Android, Linux)</span>
                                </td>
                                <td class="px-6 py-4 text-gray-600">
                                    <i class="fa-solid fa-layer-group mr-1"></i> Đa nền tảng<br>
                                    <span class="text-xs text-gray-500">(Apple, Windows, Android)</span>
                                </td>
                            </tr>
                            <tr>
                                <td class="px-6 py-4 font-medium text-gray-900">Chứng chỉ Bảo mật</td>
                                <td class="px-6 py-4 text-gray-600">SOC 2 Type II, GDPR</td>
                                <td class="px-6 py-4 text-gray-600">SOC 2 Type 2, ISO 27001</td>
                                <td class="px-6 py-4 text-gray-600">Data Privacy Framework (EU-US)</td>
                            </tr>
                            <tr>
                                <td class="px-6 py-4 font-medium text-gray-900">Quyền riêng tư</td>
                                <td class="px-6 py-4 text-gray-600">
                                    <ul class="list-disc pl-4 space-y-1">
                                        <li>Tách biệt dữ liệu mã hóa (BYOD)</li>
                                        <li>Không bán dữ liệu khách hàng</li>
                                    </ul>
                                </td>
                                <td class="px-6 py-4 text-gray-600">
                                    <ul class="list-disc pl-4 space-y-1">
                                        <li>Tuân thủ GDPR & CCPA</li>
                                        <li>Quyền người dùng (xóa/truy cập)</li>
                                    </ul>
                                </td>
                                <td class="px-6 py-4 text-gray-600">
                                    <ul class="list-disc pl-4 space-y-1">
                                        <li>Quyền được biết & không phân biệt đối xử</li>
                                        <li>Hợp đồng tiêu chuẩn (SCCs)</li>
                                    </ul>
                                </td>
                            </tr>
                            <tr>
                                <td class="px-6 py-4 font-medium text-gray-900">Tính năng Nổi bật</td>
                                <td class="px-6 py-4 text-gray-600">
                                    <span class="block mb-1 text-indigo-600 font-medium">Scripting AI</span>
                                    <span class="block text-xs">Zero-Touch Deployment, Mosyle Auth 2, Tích hợp Antivirus</span>
                                </td>
                                <td class="px-6 py-4 text-gray-600">
                                    <span class="block mb-1 text-orange-600 font-medium">Quản lý Danh tính (IAM)</span>
                                    <span class="block text-xs">JumpCloud Go (Passwordless), System Insights</span>
                                </td>
                                <td class="px-6 py-4 text-gray-600">
                                    <span class="block mb-1 text-purple-600 font-medium">Iru AI & Tuân thủ</span>
                                    <span class="block text-xs">Tự động hóa Audit, Di chuyển tự động</span>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>

        <!-- TAB 2: PRICING -->
        <div id="content-pricing" class="hidden space-y-6 animate-fade-in">
            <div class="text-center mb-8">
                <h2 class="text-2xl font-bold text-gray-900">So Sánh Mô Hình Định Giá</h2>
                <p class="text-gray-500 mt-2">Sự khác biệt lớn giữa tính theo Thiết bị và tính theo Người dùng</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                <!-- Mosyle Pricing -->
                <div class="bg-white rounded-2xl shadow-lg border-t-4 border-indigo-500 overflow-hidden transform hover:-translate-y-1 transition duration-300">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-900 flex items-center">
                            Mosyle
                            <span class="ml-2 px-2 py-1 bg-green-100 text-green-800 text-xs rounded-full">Minh bạch nhất</span>
                        </h3>
                        <p class="text-sm text-gray-500 mt-1">Định giá theo Thiết bị</p>
                        
                        <div class="mt-6 flex items-baseline">
                            <span class="text-4xl font-extrabold tracking-tight text-gray-900">$1 - $3</span>
                            <span class="ml-1 text-xl font-semibold text-gray-500">/thiết bị/tháng</span>
                        </div>
                        
                        <div class="mt-6 space-y-4">
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm"><strong>Miễn phí</strong> cho tối đa 30 thiết bị.</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Miễn phí quản lý Apple TV & Watch.</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Gói giáo dục (K-12): $5.50 - $9.00/năm.</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">MSP: Hoa hồng 100% năm đầu.</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- JumpCloud Pricing -->
                <div class="bg-white rounded-2xl shadow-lg border-t-4 border-orange-500 overflow-hidden transform hover:-translate-y-1 transition duration-300">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-900 flex items-center">
                            JumpCloud
                            <span class="ml-2 px-2 py-1 bg-blue-100 text-blue-800 text-xs rounded-full">Linh hoạt</span>
                        </h3>
                        <p class="text-sm text-gray-500 mt-1">Định giá theo Người dùng (User)</p>
                        
                        <div class="mt-6 flex items-baseline">
                            <span class="text-4xl font-extrabold tracking-tight text-gray-900">$9 - $15</span>
                            <span class="ml-1 text-xl font-semibold text-gray-500">/người/tháng</span>
                        </div>
                        
                        <div class="mt-6 space-y-4">
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Gói cơ bản từ $9, cao cấp (kèm SSO) từ $11-15.</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm"><strong>A La Carte (Mua lẻ):</strong> MDM ($5), Patch ($3), SSO ($3).</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Dùng thử miễn phí 30 ngày full tính năng.</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Iru Pricing -->
                <div class="bg-white rounded-2xl shadow-lg border-t-4 border-purple-500 overflow-hidden transform hover:-translate-y-1 transition duration-300">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-900 flex items-center">
                            Iru (Kandji)
                            <span class="ml-2 px-2 py-1 bg-gray-100 text-gray-800 text-xs rounded-full">Doanh nghiệp</span>
                        </h3>
                        <p class="text-sm text-gray-500 mt-1">Báo giá theo yêu cầu (Quote)</p>
                        
                        <div class="mt-6 flex items-baseline">
                            <span class="text-3xl font-bold tracking-tight text-gray-900">Liên hệ</span>
                        </div>
                        
                        <div class="mt-6 space-y-4">
                            <div class="flex items-start">
                                <i class="fa-solid fa-info-circle text-purple-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Giá dựa trên giải pháp và quy mô.</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Dùng thử miễn phí 14 ngày.</span>
                            </div>
                            <div class="flex items-start">
                                <i class="fa-solid fa-check text-green-500 mt-1 mr-3"></i>
                                <span class="text-gray-600 text-sm">Miễn phí dịch vụ Migration & Onboarding.</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- TAB 3: RECOMMENDATION -->
        <div id="content-recommendation" class="hidden space-y-8 animate-fade-in">
            <div class="bg-blue-50 border border-blue-200 rounded-lg p-6 text-center">
                <h2 class="text-xl font-bold text-blue-900 mb-2">Lời khuyên: Chọn MDM như chọn phương tiện di chuyển</h2>
                <p class="text-blue-800">Tùy thuộc vào "địa hình" (hạ tầng CNTT) của doanh nghiệp bạn mà lựa chọn phương tiện phù hợp.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Mosyle Analogy -->
                <div class="bg-white p-6 rounded-xl border border-gray-200 hover:shadow-lg transition text-center">
                    <div class="w-16 h-16 mx-auto bg-indigo-100 rounded-full flex items-center justify-center mb-4">
                        <i class="fa-solid fa-flag-checkered text-2xl text-indigo-600"></i>
                    </div>
                    <h3 class="text-lg font-bold text-gray-900 mb-2">Chiếc Xe Đua Chuyên Dụng</h3>
                    <p class="text-sm text-gray-600 mb-4 italic">"Tinh chỉnh riêng cho đường đua Apple"</p>
                    <p class="text-sm text-gray-600 border-t pt-4">
                        Chọn <strong>Mosyle</strong> nếu công ty bạn 100% dùng Apple. Hiệu năng cao nhất, rẻ nhất, chuyên sâu nhất.
                    </p>
                </div>

                <!-- JumpCloud Analogy -->
                <div class="bg-white p-6 rounded-xl border border-gray-200 hover:shadow-lg transition text-center">
                    <div class="w-16 h-16 mx-auto bg-orange-100 rounded-full flex items-center justify-center mb-4">
                        <i class="fa-solid fa-train-subway text-2xl text-orange-600"></i>
                    </div>
                    <h3 class="text-lg font-bold text-gray-900 mb-2">Trạm Giao Thông Công Cộng</h3>
                    <p class="text-sm text-gray-600 mb-4 italic">"Quản lý cả xe cộ và hộ chiếu (Identity)"</p>
                    <p class="text-sm text-gray-600 border-t pt-4">
                        Chọn <strong>JumpCloud</strong> nếu bạn có môi trường hỗn hợp (Win/Mac) và cần quản lý danh tính (SSO/LDAP) tập trung.
                    </p>
                </div>

                <!-- Iru Analogy -->
                <div class="bg-white p-6 rounded-xl border border-gray-200 hover:shadow-lg transition text-center">
                    <div class="w-16 h-16 mx-auto bg-purple-100 rounded-full flex items-center justify-center mb-4">
                        <i class="fa-solid fa-traffic-light text-2xl text-purple-600"></i>
                    </div>
                    <h3 class="text-lg font-bold text-gray-900 mb-2">Hệ Thống Giao Thông AI</h3>
                    <p class="text-sm text-gray-600 mb-4 italic">"Tự động điều tiết và đảm bảo tuân thủ luật lệ"</p>
                    <p class="text-sm text-gray-600 border-t pt-4">
                        Chọn <strong>Iru</strong> nếu ưu tiên hàng đầu là tự động hóa tuân thủ (Compliance) và hỗ trợ AI cho đa nền tảng.
                    </p>
                </div>
            </div>
        </div>

    </main>

    <script>
        function switchTab(tabName) {
            // Hide all contents
            document.getElementById('content-overview').classList.add('hidden');
            document.getElementById('content-pricing').classList.add('hidden');
            document.getElementById('content-recommendation').classList.add('hidden');

            // Reset tab styles
            const tabs = ['overview', 'pricing', 'recommendation'];
            tabs.forEach(t => {
                const btn = document.getElementById(`tab-${t}`);
                btn.classList.remove('tab-active', 'border-b-2', 'border-blue-600', 'text-blue-600');
                btn.classList.add('tab-inactive', 'border-transparent');
            });

            // Show selected content
            document.getElementById(`content-${tabName}`).classList.remove('hidden');

            // Highlight selected tab
            const activeBtn = document.getElementById(`tab-${tabName}`);
            activeBtn.classList.remove('tab-inactive', 'border-transparent');
            activeBtn.classList.add('tab-active', 'border-blue-600', 'text-blue-600');
        }
    </script>
</body>
</html><img width="1161" height="745" alt="image" src="https://github.com/user-attachments/assets/e37b89d6-b67c-4b22-827d-5d6bda3d4541" />
