import React from 'react';

export default function CommonKADSAnalysis() {
  return (
    <div className="w-full h-full bg-gradient-to-br from-slate-50 to-blue-50 p-8 overflow-auto">
      <div className="max-w-7xl mx-auto">
        <h1 className="text-4xl font-bold text-center mb-4 text-slate-800">
          華語課程 LLM 代理人系統
        </h1>
        <h2 className="text-2xl text-center mb-8 text-gray-600">
          CommonKADS 模型分析
        </h2>

        {/* Organization Model */}
        <div className="bg-white rounded-xl shadow-2xl p-8 mb-8">
          <div className="flex items-center mb-6">
            <div className="bg-blue-500 text-white w-12 h-12 rounded-full flex items-center justify-center text-2xl font-bold mr-4">
              O
            </div>
            <h2 className="text-3xl font-bold text-blue-700">Organization Model（組織模型）</h2>
          </div>

          {/* OM-1 */}
          <div className="mb-6 bg-blue-50 p-6 rounded-lg border-l-4 border-blue-500">
            <h3 className="text-xl font-bold mb-4 text-blue-800">OM-1: 組織問題與機會</h3>
            <div className="grid grid-cols-2 gap-4">
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-2">問題識別</h4>
                <ul className="text-sm text-gray-700 space-y-1">
                  <li>• 教師工作負擔過重（批改、出題）</li>
                  <li>• 學生缺乏個性化學習路徑</li>
                  <li>• 無法即時掌握學習成效</li>
                  <li>• 教材利用率低，重複製作內容</li>
                  <li>• 缺乏系統化的學習歷程追蹤</li>
                </ul>
              </div>
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-2">解決方案</h4>
                <ul className="text-sm text-gray-700 space-y-1">
                  <li>• 導入 LLM 代理人自動化系統</li>
                  <li>• 建立學習歷程管理機制</li>
                  <li>• 開發智能試題生成功能</li>
                  <li>• 實現個性化學習目標制定</li>
                  <li>• 整合現有教材資源</li>
                </ul>
              </div>
            </div>
          </div>

          {/* OM-2 */}
          <div className="mb-6 bg-blue-50 p-6 rounded-lg border-l-4 border-blue-500">
            <h3 className="text-xl font-bold mb-4 text-blue-800">OM-2: 組織結構</h3>
            <div className="bg-white p-4 rounded-lg shadow">
              <svg viewBox="0 0 800 250" className="w-full">
                <rect x="325" y="20" width="150" height="50" fill="#3b82f6" stroke="#1e40af" strokeWidth="2" rx="5"/>
                <text x="400" y="50" textAnchor="middle" fill="white" fontSize="16" fontWeight="bold">華語教學單位</text>
                
                <line x1="400" y1="70" x2="400" y2="100" stroke="#64748b" strokeWidth="2"/>
                <line x1="150" y1="100" x2="650" y2="100" stroke="#64748b" strokeWidth="2"/>
                <line x1="150" y1="100" x2="150" y2="120" stroke="#64748b" strokeWidth="2"/>
                <line x1="400" y1="100" x2="400" y2="120" stroke="#64748b" strokeWidth="2"/>
                <line x1="650" y1="100" x2="650" y2="120" stroke="#64748b" strokeWidth="2"/>
                
                <rect x="75" y="120" width="150" height="50" fill="#10b981" stroke="#059669" strokeWidth="2" rx="5"/>
                <text x="150" y="150" textAnchor="middle" fill="white" fontSize="14" fontWeight="bold">教師群組</text>
                
                <rect x="325" y="120" width="150" height="50" fill="#8b5cf6" stroke="#6d28d9" strokeWidth="2" rx="5"/>
                <text x="400" y="150" textAnchor="middle" fill="white" fontSize="14" fontWeight="bold">LLM 代理人系統</text>
                
                <rect x="575" y="120" width="150" height="50" fill="#ef4444" stroke="#b91c1c" strokeWidth="2" rx="5"/>
                <text x="650" y="150" textAnchor="middle" fill="white" fontSize="14" fontWeight="bold">學生群組</text>
                
                <line x1="400" y1="170" x2="400" y2="190" stroke="#64748b" strokeWidth="2"/>
                
                <rect x="250" y="190" width="120" height="40" fill="#ec4899" stroke="#be185d" strokeWidth="2" rx="5"/>
                <text x="310" y="215" textAnchor="middle" fill="white" fontSize="12" fontWeight="bold">學習歷程系統</text>
                
                <rect x="430" y="190" width="120" height="40" fill="#3b82f6" stroke="#1e40af" strokeWidth="2" rx="5"/>
                <text x="490" y="215" textAnchor="middle" fill="white" fontSize="12" fontWeight="bold">教材管理系統</text>
              </svg>
            </div>
          </div>

          {/* OM-3 */}
          <div className="mb-6 bg-blue-50 p-6 rounded-lg border-l-4 border-blue-500">
            <h3 className="text-xl font-bold mb-4 text-blue-800">OM-3: 流程分析（對應 UML 6 個階段）</h3>
            <div className="space-y-3">
              <div className="bg-white p-4 rounded-lg shadow">
                <div className="flex items-center mb-2">
                  <span className="bg-amber-500 text-white px-3 py-1 rounded-full text-sm font-bold mr-3">P1</span>
                  <h4 className="font-bold text-gray-800">課程設定流程</h4>
                </div>
                <p className="text-sm text-gray-700 ml-12">教師上傳教材 → 系統整理 → 設定目標 → LLM 載入教材</p>
              </div>
              
              <div className="bg-white p-4 rounded-lg shadow">
                <div className="flex items-center mb-2">
                  <span className="bg-blue-500 text-white px-3 py-1 rounded-full text-sm font-bold mr-3">P2</span>
                  <h4 className="font-bold text-gray-800">學生登入流程</h4>
                </div>
                <p className="text-sm text-gray-700 ml-12">學生登入 → 載入學習歷程 → LLM 分析程度</p>
              </div>
              
              <div className="bg-white p-4 rounded-lg shadow">
                <div className="flex items-center mb-2">
                  <span className="bg-amber-500 text-white px-3 py-1 rounded-full text-sm font-bold mr-3">P3</span>
                  <h4 className="font-bold text-gray-800">目標制定流程</h4>
                </div>
                <p className="text-sm text-gray-700 ml-12">整合歷程 → 分析弱點 → 制定目標 → 呈現給學生</p>
              </div>
              
              <div className="bg-white p-4 rounded-lg shadow">
                <div className="flex items-center mb-2">
                  <span className="bg-indigo-500 text-white px-3 py-1 rounded-full text-sm font-bold mr-3">P4</span>
                  <h4 className="font-bold text-gray-800">試題生成流程</h4>
                </div>
                <p className="text-sm text-gray-700 ml-12">請求試題 → 獲取教材 → 查詢弱點 → 生成試題 → 呈現給學生</p>
              </div>
              
              <div className="bg-white p-4 rounded-lg shadow">
                <div className="flex items-center mb-2">
                  <span className="bg-pink-500 text-white px-3 py-1 rounded-full text-sm font-bold mr-3">P5</span>
                  <h4 className="font-bold text-gray-800">評估流程</h4>
                </div>
                <p className="text-sm text-gray-700 ml-12">學生作答 → LLM 批改 → 分析錯誤 → 記錄歷程 → 呈現報告</p>
              </div>
              
              <div className="bg-white p-4 rounded-lg shadow">
                <div className="flex items-center mb-2">
                  <span className="bg-green-500 text-white px-3 py-1 rounded-full text-sm font-bold mr-3">P6</span>
                  <h4 className="font-bold text-gray-800">監控流程</h4>
                </div>
                <p className="text-sm text-gray-700 ml-12">教師查看報告 → 分析學生表現 → 調整教學策略</p>
              </div>
            </div>
          </div>

          {/* OM-4 */}
          <div className="mb-6 bg-blue-50 p-6 rounded-lg border-l-4 border-blue-500">
            <h3 className="text-xl font-bold mb-4 text-blue-800">OM-4: 知識資產</h3>
            <div className="grid grid-cols-2 gap-4">
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-3">內隱知識</h4>
                <ul className="text-sm text-gray-700 space-y-1">
                  <li>• 教師的教學經驗與技巧</li>
                  <li>• 學生常見錯誤模式判斷</li>
                  <li>• 難度評估與調整經驗</li>
                  <li>• 個別學生學習特性理解</li>
                  <li>• 華語教學法知識</li>
                </ul>
              </div>
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-3">外顯知識</h4>
                <ul className="text-sm text-gray-700 space-y-1">
                  <li>• 現有華語教材內容</li>
                  <li>• 學習歷程數據記錄</li>
                  <li>• 試題題庫與答案</li>
                  <li>• 評分標準與規則</li>
                  <li>• 課程大綱與目標</li>
                </ul>
              </div>
            </div>
          </div>

          {/* OM-5 */}
          <div className="bg-blue-50 p-6 rounded-lg border-l-4 border-blue-500">
            <h3 className="text-xl font-bold mb-4 text-blue-800">OM-5: 可行性評估</h3>
            <div className="grid grid-cols-3 gap-4">
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-2">💰 經濟可行性</h4>
                <p className="text-sm text-gray-700 mb-2">成本效益分析：</p>
                <ul className="text-xs text-gray-600 space-y-1">
                  <li>✓ 減少 80% 重複工作</li>
                  <li>✓ 利用現有教材資源</li>
                  <li>✓ LLM API 成本可控</li>
                  <li>✓ 提升教學效率 3-5 倍</li>
                </ul>
              </div>
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-2">⚙️ 技術可行性</h4>
                <p className="text-sm text-gray-700 mb-2">技術需求：</p>
                <ul className="text-xs text-gray-600 space-y-1">
                  <li>✓ LLM API 整合</li>
                  <li>✓ 學習歷程資料庫</li>
                  <li>✓ 教材管理系統</li>
                  <li>✓ Web 介面開發</li>
                </ul>
              </div>
              <div className="bg-white p-4 rounded-lg shadow">
                <h4 className="font-bold text-blue-700 mb-2">👥 組織可行性</h4>
                <p className="text-sm text-gray-700 mb-2">接受度評估：</p>
                <ul className="text-xs text-gray-600 space-y-1">
                  <li>✓ 減輕教師負擔高接受</li>
                  <li>✓ 學生喜愛即時回饋</li>
                  <li>✓ 管理層支持創新</li>
                  <li>✓ 符合教育數位化趨勢</li>
                </ul>
              </div>
            </div>
          </div>
        </div>

        {/* Task Model */}
        <div className="bg-white rounded-xl shadow-2xl p-8 mb-8">
          <div className="flex items-center mb-6">
            <div className="bg-green-500 text-white w-12 h-12 rounded-full flex items-center justify-center text-2xl font-bold mr-4">
              T
            </div>
            <h2 className="text-3xl font-bold text-green-700">Task Model（任務模型）</h2>
          </div>

          {/* 任務分解 */}
          <div className="mb-6">
            <h3 className="text-xl font-bold mb-4 text-green-800">任務階層結構（TM-1）</h3>
            <div className="bg-green-50 p-6 rounded-lg">
              <div className="space-y-4">
                {/* 主任務 */}
                <div className="bg-white p-4 rounded-lg shadow-md border-l-4 border-green-600">
                  <div className="font-bold text-lg text-green-900 mb-2">主任務：提升華語學習成效</div>
                  
                  {/* 子任務 */}
                  <div className="ml-6 mt-3 space-y-3">
                    <div className="bg-amber-50 p-3 rounded-lg border-l-4 border-amber-500">
                      <div className="font-bold text-amber-900">T1: 教材管理任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T1.1: 上傳教材</li>
                        <li>• T1.2: 整理教材內容</li>
                        <li>• T1.3: 設定教學目標</li>
                        <li>• T1.4: 教材內容索引化</li>
                      </ul>
                    </div>

                    <div className="bg-blue-50 p-3 rounded-lg border-l-4 border-blue-500">
                      <div className="font-bold text-blue-900">T2: 學習歷程管理任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T2.1: 載入學生歷程資料</li>
                        <li>• T2.2: 分析學習狀況</li>
                        <li>• T2.3: 記錄學習數據</li>
                        <li>• T2.4: 更新能力評估</li>
                      </ul>
                    </div>

                    <div className="bg-amber-50 p-3 rounded-lg border-l-4 border-amber-600">
                      <div className="font-bold text-amber-900">T3: 學習目標制定任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T3.1: 整合歷程數據</li>
                        <li>• T3.2: 識別強項與弱點</li>
                        <li>• T3.3: 制定短中期目標</li>
                        <li>• T3.4: 呈現學習目標給學生</li>
                      </ul>
                    </div>

                    <div className="bg-indigo-50 p-3 rounded-lg border-l-4 border-indigo-500">
                      <div className="font-bold text-indigo-900">T4: 試題生成任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T4.1: 接收試題請求</li>
                        <li>• T4.2: 查詢相關教材</li>
                        <li>• T4.3: 分析學生弱點</li>
                        <li>• T4.4: 生成個性化試題</li>
                        <li>• T4.5: 呈現試題給學生</li>
                      </ul>
                    </div>

                    <div className="bg-pink-50 p-3 rounded-lg border-l-4 border-pink-500">
                      <div className="font-bold text-pink-900">T5: 評估與回饋任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T5.1: 接收學生答案</li>
                        <li>• T5.2: 批改與評分</li>
                        <li>• T5.3: 分析錯誤類型</li>
                        <li>• T5.4: 生成評估報告</li>
                        <li>• T5.5: 記錄到學習歷程</li>
                      </ul>
                    </div>

                    <div className="bg-purple-50 p-3 rounded-lg border-l-4 border-purple-500">
                      <div className="font-bold text-purple-900">T6: 互動學習任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T6.1: 接收學生問題</li>
                        <li>• T6.2: 理解問題意圖</li>
                        <li>• T6.3: 查詢相關知識</li>
                        <li>• T6.4: 生成個性化回應</li>
                        <li>• T6.5: 記錄互動數據</li>
                      </ul>
                    </div>

                    <div className="bg-green-50 p-3 rounded-lg border-l-4 border-green-600">
                      <div className="font-bold text-green-900">T7: 報告生成任務</div>
                      <ul className="text-sm text-gray-700 mt-2 space-y-1">
                        <li>• T7.1: 彙整學習數據</li>
                        <li>• T7.2: 生成視覺化報告</li>
                        <li>• T7.3: 識別需關注學生</li>
                        <li>• T7.4: 提供教學建議</li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          {/* 知識密集任務 */}
          <div className="mb-6">
            <h3 className="text-xl font-bold mb-4 text-green-800">知識密集任務分析（TM-2）</h3>
            <div className="grid grid-cols-2 gap-4">
              <div className="bg-green-50 p-4 rounded-lg">
                <h4 className="font-bold text-green-800 mb-3">高度知識密集任務</h4>
                <div className="space-y-2 text-sm">
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-green-700">T3: 目標制定</span>
                    <p className="text-gray-600 text-xs mt-1">需要教學經驗與學習理論知識</p>
                  </div>
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-green-700">T4: 試題生成</span>
                    <p className="text-gray-600 text-xs mt-1">需要教材理解與難度控制</p>
                  </div>
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-green-700">T5: 評估回饋</span>
                    <p className="text-gray-600 text-xs mt-1">需要錯誤分析與教學診斷</p>
                  </div>
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-green-700">T6: 互動學習</span>
                    <p className="text-gray-600 text-xs mt-1">需要語言理解與教學策略</p>
                  </div>
                </div>
              </div>
              
              <div className="bg-gray-50 p-4 rounded-lg">
                <h4 className="font-bold text-gray-800 mb-3">一般知識任務</h4>
                <div className="space-y-2 text-sm">
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-gray-700">T1: 教材管理</span>
                    <p className="text-gray-600 text-xs mt-1">主要是資料處理與組織</p>
                  </div>
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-gray-700">T2: 歷程管理</span>
                    <p className="text-gray-600 text-xs mt-1">資料庫操作與記錄管理</p>
                  </div>
                  <div className="bg-white p-3 rounded shadow">
                    <span className="font-semibold text-gray-700">T7: 報告生成</span>
                    <p className="text-gray-600 text-xs mt-1">資料彙整與視覺化呈現</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        {/* Agent Model */}
        <div className="bg-white rounded-xl shadow-2xl p-8 mb-8">
          <div className="flex items-center mb-6">
            <div className="bg-purple-500 text-white w-12 h-12 rounded-full flex items-center justify-center text-2xl font-bold mr-4">
              A
            </div>
            <h2 className="text-3xl font-bold text-purple-700">Agent Model（代理人模型）</h2>
          </div>

          {/* 代理人識別 */}
          <div className="mb-6">
            <h3 className="text-xl font-bold mb-4 text-purple-800">代理人識別與特性（AM-1）</h3>
            <div className="grid grid-cols-2 gap-6">
              {/* 學生代理人 */}
              <div className="bg-red-50 p-5 rounded-lg border-2 border-red-300">
                <div className="flex items-center mb-3">
                  <div className="bg-red-500 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold mr-3">
                    S
                  </div>
                  <h4 className="font-bold text-red-900 text-lg">學生（Student Agent）</h4>
                </div>
                <div className="space-y-2 text-sm">
                  <div>
                    <span className="font-semibold text-red-800">角色：</span>
                    <span className="text-gray-700">學習者、任務請求者</span>
                  </div>
                  <div>
                    <span className="font-semibold text-red-800">能力：</span>
                    <ul className="text-gray-700 ml-4 mt-1">
                      <li>• 提出問題與需求</li>
                      <li>• 完成練習與試題</li>
                      <li>• 接收回饋與建議</li>
                    </ul>
                  </div>
                  <div>
                    <span className="font-semibold text-red-800">目標：</span>
                    <span className="text-gray-700">提升華語能力</span>
                  </div>
                </div>
              </div>

              {/* LLM 代理人 */}
              <div className="bg-purple-50 p-5 rounded-lg border-2 border-purple-300">
                <div className="flex items-center mb-3">
                  <div className="bg-purple-500 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold mr-3">
                    L
                  </div>
                  <h4 className="font-bold text-purple-900 text-lg">LLM 代理人（LLM Agent）</h4>
                </div>
                <div className="space-y-2 text-sm">
                  <div>
                    <span className="font-semibold text-purple-800">角色：</span>
                    <span className="text-gray-700">智能教學助理、核心處理者</span>
                  </div>
                  <div>
                    <span className="font-semibold text-purple-800">能力：</span>
                    <ul className="text-gray-700 ml-4 mt-1">
                      <li>• 理解自然語言問題</li>
                      <li>• 生成個性化內容</li>
                      <li>• 分析學習數據</li>
                      <li>• 制定學習策略</li>
                      <li>• 評估學習成效</li>
                    </ul>
                  </div>
                  <div>
                    <span className="font-semibold text-purple-800">目標：</span>
                    <span className="text-gray-700">提供個性化教學支援</span>
                  </div>
                </div>
              </div>

              {/* 教師代理人 */}
              <div className="bg-green-50 p-5 rounded-lg border-2 border-green-300">
                <div className="flex items-center mb-3">
                  <div className="bg-green-500 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold mr-3">
                    T
                  </div>
                  <h4 className="font-bold text-green-900 text-lg">教師（Teacher Agent）</h4>
                </div>
                <div className="space-y-2 text-sm">
                  <div>
                    <span className="font-semibold text-green-800">角色：</span>
                    <span className="text-gray-700">教學管理者、監督者</span>
                  </div>
                  <div>
                    <span className="font-semibold text-green-800">能力：</span>
                    <ul className="text-gray-700 ml-4 mt-1">
                      <li>• 上傳與管理教材</li>
                      <li>• 設定教學目標</li>
                      <li>• 監控學習進度</li>
                      <li>• 查看學習報告</li>
                      <li>• 調整教學策略</li>
                    </ul>
                  </div>
                  <div>
                    <span className="font-semibold text-green-800">目標：</span>
                    <span className="text-gray-700">優化教學品質、減輕負擔</span>
                  </div>
                </div>
              </div>

              {/* 學習歷程系統 */}
              <div className="bg-pink-50 p-5 rounded-lg border-2 border-pink-300">
                <div className="flex items-center mb-3">
                  <div className="bg-pink-500 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold mr-3">
                    P
                  </div>
                  <h4 className="font-bold text-pink-900 text-lg">學習歷程系統</h4>
                </div>
                <div className="space-y-2 text-sm">
                  <div>
                    <span className="font-semibold text-pink-800">角色：</span>
                    <span className="text-gray-700">資料管理者</span>
                  </div>
                  <div>
                    <span className="font-semibold text-pink-800">能力：</span>
                    <ul className="text-gray-700 ml-4 mt-1">
                      <li>• 儲存學習記錄</li>
                      <li>• 提供歷程查詢</li>
                      <li>• 更新能力評估</li>
                    </ul>
                  </div>
                  <div>
                    <span className="font-semibold text-pink-800">目標：</span>
                    <span className="text-gray-700">完整記錄學習歷程</span>
                  </div>
                </div>
              </div>

              {/* 教材系統 */}
              <div className="bg-blue-50 p-5 rounded-lg border-2 border-blue-300">
                <div className="flex items-center mb-3">
                  <div className="bg-blue-500 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold mr-3">
                    M
                  </div>
                  <h4 className="font-bold text-blue-900 text-lg">教材系統</h4>
                </div>
                <div className="space-y-2 text-sm">
                  <div>
                    <span className="font-semibold text-blue-800">角色：</span>
                    <span className="text-gray-700">內容提供者</span>
                  </div>
                  <div>
                    <span className="font-semibold text-blue-800">能力：</span>
                    <ul className="text-gray-700 ml-4 mt-1">
                      <li>• 儲存教材內容</li>
                      <li>• 索引與檢索</li>
                      <li>• 提供教材查詢</li>
                    </ul>
                  </div>
                  <div>
                    <span className="font-semibold text-blue-800">目標：</span>
                    <span className="text-gray-700">管理教學資源</span>
                  </div>
                </div>
              </div>
            </div>
          </div>

          {/* 代理人任務分配表 */}
          <div>
            <h3 className="text-xl font-bold mb-4 text-purple-800">代理人任務分配（AM-3）</h3>
            <div className="overflow-x-auto">
              <table className="w-full text-sm border-collapse">
                <thead>
                  <tr className="bg-purple-600 text-white">
                    <th className="border border-purple-700 p-3 text-left">任務</th>
                    <th className="border border-purple-700 p-3 text-center">學生</th>
                    <th className="border border-purple-700 p-3 text-center">LLM</th>
                    <th className="border border-purple-700 p-3 text-center">歷程</th>
                    <th className="border border-purple-700 p-3 text-center">教材</th>
                    <th className="border border-purple-700 p-3 text-center">教師</th>
                  </tr>
                </thead>
                <tbody className="bg-white">
                  <tr>
                    <td className="border border-gray-300 p-3">T1: 教材管理</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">協助</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center bg-blue-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center bg-green-100">發起</td>
                  </tr>
                  <tr>
                    <td className="border border-gray-300 p-3">T2: 歷程管理</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">協助</td>
                    <td className="border border-gray-300 p-3 text-center bg-pink-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                  </tr>
                  <tr>
                    <td className="border border-gray-300 p-3">T3: 目標制定</td>
                    <td className="border border-gray-300 p-3 text-center bg-red-100">接收</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center bg-pink-100">提供</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                  </tr>
                  <tr>
                    <td className="border border-gray-300 p-3">T4: 試題生成</td>
                    <td className="border border-gray-300 p-3 text-center bg-red-100">請求</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center bg-pink-100">提供</td>
                    <td className="border border-gray-300 p-3 text-center bg-blue-100">提供</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                  </tr>
                  <tr>
                    <td className="border border-gray-300 p-3">T5: 評估回饋</td>
                    <td className="border border-gray-300 p-3 text-center bg-red-100">提交</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center bg-pink-100">記錄</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                  </tr>
                  <tr>
                    <td className="border border-gray-300 p-3">T6: 互動學習</td>
                    <td className="border border-gray-300 p-3 text-center bg-red-100">提問</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center bg-pink-100">參考</td>
                    <td className="border border-gray-300 p-3 text-center bg-blue-100">提供</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                  </tr>
                  <tr>
                    <td className="border border-gray-300 p-3">T7: 報告生成</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center bg-purple-100">主責</td>
                    <td className="border border-gray-300 p-3 text-center bg-pink-100">提供</td>
                    <td className="border border-gray-300 p-3 text-center">-</td>
                    <td className="border border-gray-300 p-3 text-center bg-green-100">查看</td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </div>

        {/* 總結 */}
        <div className="bg-gradient-to-r from-indigo-100 to-purple-100 rounded-xl shadow-xl p-8">
          <h2 className="text-2xl font-bold mb-6 text-indigo-900 text-center">📊 CommonKADS 模型整合總結</h2>
          <div className="grid grid-cols-3 gap-6">
            <div className="bg-white p-6 rounded-lg shadow-lg">
              <div className="text-4xl text-center mb-3">🏢</div>
              <h3 className="font-bold text-blue-900 text-center mb-3">Organization Model</h3>
              <p className="text-sm text-gray-700 text-center">定義華語教學單位的問題、流程、知識資產，評估系統可行性</p>
            </div>
            <div className="bg-white p-6 rounded-lg shadow-lg">
              <div className="text-4xl text-center mb-3">📋</div>
              <h3 className="font-bold text-green-900 text-center mb-3">Task Model</h3>
              <p className="text-sm text-gray-700 text-center">分解 7 大任務，識別知識密集點，規劃任務執行流程</p>
            </div>
            <div className="bg-white p-6 rounded-lg shadow-lg">
              <div className="text-4xl text-center mb-3">🤖</div>
              <h3 className="font-bold text-purple-900 text-center mb-3">Agent Model</h3>
              <p className="text-sm text-gray-700 text-center">定義 5 個代理人角色、能力、互動方式與任務分配</p>
            </div>
          </div>
          
          <div className="mt-8 bg-white p-6 rounded-lg shadow-lg">
            <h3 className="font-bold text-indigo-900 text-lg mb-4 text-center">🎯 系統核心價值鏈</h3>
            <div className="flex items-center justify-center flex-wrap gap-4 text-sm">
              <div className="bg-blue-100 px-4 py-2 rounded-lg font-semibold text-blue-900">組織問題識別</div>
              <span className="text-2xl">→</span>
              <div className="bg-green-100 px-4 py-2 rounded-lg font-semibold text-green-900">任務分解執行</div>
              <span className="text-2xl">→</span>
              <div className="bg-purple-100 px-4 py-2 rounded-lg font-semibold text-purple-900">代理人協作</div>
              <span className="text-2xl">→</span>
              <div className="bg-red-100 px-4 py-2 rounded-lg font-semibold text-red-900">提升學習成效</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
}
